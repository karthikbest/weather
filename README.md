/* Base visibility toggles */
.mobile-only {
  display: none;
}

.desktop-only {
  display: block;
}

@media (max-width: 768px) {
  .mobile-only {
    display: block;
    margin: 1rem 0;
  }

  .desktop-only {
    display: none;
  }

  .AccordionRoot {
    border: 1px solid #ccc;
    border-radius: 6px;
  }

  .AccordionItem {
    overflow: hidden;
    border-bottom: 1px solid #ddd;
  }

  .AccordionHeader {
    display: flex;
  }

  .AccordionTrigger {
    all: unset;
    background-color: #f9f9f9;
    font-weight: bold;
    padding: 1rem;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
  }

  .AccordionContent {
    padding: 0.5rem 1rem;
    animation: slideDown 300ms ease;
  }

  .arrow {
    transition: transform 0.3s ease;
  }

  [data-state='open'] .arrow {
    transform: rotate(180deg);
  }

  .TabsList {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }

  .TabsTrigger {
    background: white;
    border: none;
    text-align: left;
    padding: 0.75rem 1rem;
    border-left: 4px solid transparent;
  }

  .TabsTrigger[data-state='active'] {
    border-left-color: #0074cc;
    background-color: #eef6ff;
  }
}

/* Shared styling for tab content */
.TabsContent {
  padding: 1rem;
}