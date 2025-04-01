@media (max-width: 768px) {
  .mobile-only {
    display: block;
    margin: 1rem;
  }

  .AccordionRoot {
    border: 1px solid #ddd;
    border-radius: 8px;
    background-color: #fff;
  }

  .AccordionItem {
    border-bottom: 1px solid #eee;
  }

  .AccordionTrigger {
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

  .AccordionContent {
    padding: 0.5rem 1rem;
    animation: slideDown 300ms ease;
    border-top: 1px solid #ddd;
  }

  .TabsList {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    padding: 0.5rem 0;
  }

  .TabsTrigger {
    background: transparent;
    border: none;
    text-align: left;
    font-size: 1rem;
    font-weight: 500;
    padding: 0.75rem 1rem;
    border-left: 4px solid transparent;
    transition: background 0.2s;
  }

  .TabsTrigger[data-state="active"] {
    border-left-color: #0074cc;
    background-color: #eef6ff;
  }

  .arrow {
    transition: transform 0.3s ease;
    font-size: 1.25rem;
  }

  [data-state='open'] .arrow {
    transform: rotate(180deg);
  }

  /* Optional: add heading above accordion */
  .mobileSettingsHeading {
    font-size: 1.25rem;
    font-weight: bold;
    margin-bottom: 0.5rem;
    padding: 0 0.5rem;
  }
}

@media (min-width: 769px) {
  .mobile-only {
    display: none;
  }
}