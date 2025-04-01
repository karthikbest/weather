@media (min-width: 769px) {
  /* Tabs Layout */
  .tabsList {
    display: flex;
    justify-content: flex-start;
    border-bottom: 2px solid #ccc;
    padding-left: 1rem;
    margin-bottom: 1.5rem;
  }

  .tabsTrigger {
    background: none;
    border: none;
    font: inherit;
    padding: 1rem;
    margin-right: 1.5rem;
    border-bottom: 2px solid transparent;
    cursor: pointer;
    font-weight: 500;
  }

  .tabsTrigger[data-state="active"] {
    border-bottom: 2px solid #0074cc; /* Blue underline for active tab */
    font-weight: 600;
  }

  /* Profile header background block */
  .profileHeaderSection {
    background-color: #003a6d; /* Dark blue */
    padding: 2rem 1rem;
    position: relative;
  }

  .myProfileData {
    background: white;
    padding: 1rem 1.5rem;
    border-radius: 6px;
    box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
    display: flex;
    align-items: center;
    gap: 1rem;
    position: relative;
    top: -2.5rem; /* pulls it up into the blue section */
    margin: 0 1rem;
  }

  .myProfilePhoto {
    width: 64px;
    height: 64px;
    border-radius: 50%;
    background-color: #e0e0e0;
    font-weight: bold;
    font-size: 1.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .myProfileDisplayName {
    font-weight: bold;
    font-size: 1rem;
  }

  .myProfileEmailText {
    font-size: 0.9rem;
    color: #555;
  }

  /* Optional: tighten spacing */
  .tabsContent {
    padding-top: 1rem;
  }
}