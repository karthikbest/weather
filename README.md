@media (min-width: 769px) {
  .tabsList {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    border-bottom: 2px solid #ccc;
    padding-left: 1rem;
    gap: 1.5rem; /* spacing between tabs */
    margin-bottom: 1.5rem;
  }

  .tabsTrigger {
    background: none;
    border: none;
    font: inherit;
    padding: 0.5rem 0;
    margin: 0;
    border-bottom: 3px solid transparent;
    cursor: pointer;
    font-weight: 600;
    color: #000;
  }

  .tabsTrigger[data-state="active"] {
    border-bottom: 3px solid #0074cc; /* strong blue underline */
    color: #000;
  }
}