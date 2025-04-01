@media (min-width: 769px) {
  .tabsList {
    display: flex;
    border-bottom: 2px solid #d3d3d3;
    margin: 0;
    padding: 0;
  }

  .tabsTrigger {
    flex: 1;
    text-align: center;
    background: none;
    border: none;
    font: inherit;
    padding: 0.75rem 0;
    font-weight: 600;
    border-bottom: 3px solid transparent;
    cursor: pointer;
    transition: border-color 0.2s ease;
  }

  .tabsTrigger[data-state="active"] {
    border-bottom-color: #0074cc; /* Blue underline */
  }
}