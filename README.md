@media (max-width: 768px) {
  /* Stack the tab buttons vertically */
  [role="tablist"] {
    flex-direction: column !important;
    align-items: stretch;
    border-bottom: none;
    border-right: 1px solid #ccc;
    padding-right: 1rem;
    gap: 0.5rem;
  }

  [role="tab"] {
    width: 100%;
    text-align: left;
    border: none;
    border-left: 4px solid transparent;
    padding: 0.75rem 1rem;
    font-weight: bold;
    background-color: #f9f9f9;
  }

  [role="tab"][data-state="active"] {
    border-left-color: #0074cc; /* highlight active tab */
    background-color: #eef6ff;
  }

  /* Make tab content full width and stack underneath */
  [role="tabpanel"] {
    width: 100%;
    padding: 1rem;
    border-top: 1px solid #ddd;
    margin-top: 1rem;
  }

  /* Optional: container styling for clarity */
  .TabsRoot {
    display: flex;
    flex-direction: column;
  }

  .TabsList {
    display: flex;
  }
}