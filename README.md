.radix-tabs-trigger[data-state='active']::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 80%; /* or 100% */
  height: 8px; /* slightly taller */
  background-color: #005DAA;
  border-radius: 4px; /* must be at least half the height */
  overflow: visible;
}