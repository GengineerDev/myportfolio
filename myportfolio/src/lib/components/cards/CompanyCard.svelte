<script>
    export let imgPath = "/icons/TENTEN.png";
    export let companyName = "Default Company Name";
  </script>
  
  <style>
    .company-card {
      display: flex;
      justify-content: center;
      border-radius: 20px 96px 20px 20px;
      border: 4px solid var(--pantone-orange);
      width: 377px;
      max-width: 377px;
      padding: 56px 48px;
    }
  </style>
  
  <div class="company-card">
    <div>
      <img src={imgPath} alt={companyName + " logo"} height="50px" />
      <p class="subheadings-1 gradient-text-background">{companyName}</p>
    </div>
  </div>