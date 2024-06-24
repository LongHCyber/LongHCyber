# My Profile

<div style="font-size: 24px; font-weight: bold;">
  <p id="line1">My Name</p>
  <p id="line2">Job</p>
</div>

<style>
  @keyframes move {
    0% { transform: translateX(0); }
    50% { transform: translateX(100px); }
    100% { transform: translateX(0); }
  }

  @keyframes fade {
    0% { opacity: 1; }
    50% { opacity: 0; }
    100% { opacity: 1; }
  }

  #line1 {
    animation: move 5s infinite;
  }

  #line2 {
    animation: fade 5s infinite;
  }
</style>
