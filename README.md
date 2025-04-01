/* Show/hide based on screen size */
.mobile-only {
  display: none;
}
.desktop-only {
  display: block;
}

@media (max-width: 768px) {
  .mobile-only {
    display: block;
  }
  .desktop-only {
    display: none;
  }

  .accordionRoot {
    border: 1px solid #ddd;
    border-radius: 8px;
    background-color: #fff;
  }

  .accordionItem {
    border-bottom: 1px solid #eee;
  }

  .accordionTrigger {
    all: unset;
    width: 100%;
    background-color: #f5f5f5;
    padding: 1rem;
    font-size: 1rem;
    font-weight: 600;
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
    border-bottom: 1px solid #ccc;
  }

  .accordionContent {
    padding: 0.5rem 1rem;
    animation: slideDown 300ms ease;
    border-top: 1px solid #ddd;
  }

  .arrow {
    transition: transform 0.3s ease;
    font-size: 1.25rem;
  }

  [data-state='open'] .arrow {
    transform: rotate(180deg);
  }
}

/* Shared styling for Tabs */
.tabsList {
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  gap: 1rem;
  padding: 0.5rem 0;
}

.tabsTrigger {
  background: transparent;
  border: none;
  padding: 0.5rem 1rem;
  font: inherit;
  border-bottom: 2px solid transparent;
  cursor: pointer;
}

.tabsTrigger[data-state="active"] {
  border-bottom-color: #0074cc; /* blue underline */
  font-weight: 600;
}

.tabsTrigger[data-state="inactive"] {
  border-bottom-color: transparent;
}

.tabsContent {
  padding: 1rem 0;
}

/* Optional: heading */
.settingsHeading {
  font-size: 1.25rem;
  font-weight: bold;
  margin: 1rem 0 0.5rem 0;
}