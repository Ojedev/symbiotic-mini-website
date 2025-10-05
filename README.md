<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Symbiotic Mini</title>
</head>
<link rel="stylesheet" href="practice.css">

<body>

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Symbiotic Protocol</title>
  <style>
    /* === Reset & Fonts === */
    * {
      margin: 0; padding: 0;
      box-sizing: border-box;
      font-family: "Segoe UI", Arial, sans-serif;
    }
    body {
      background-color: #0a0a0f;
      color: #eee;
      line-height: 1.6;
    }
    a { color: #94fc86; text-decoration: none; }
    a:hover { text-decoration: none;
      }

    /* === Navbar === */
    header {
      background: #111;
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    nav ul {
      list-style: none;
        display: flex;
        gap: 1.5rem;
    }
    nav ul li a {
      font-weight: bold;
      transform: scale(1.3);
      color: #25a822;
    }
    nav ul li a :hover{
       text-decoration: none;
       background-color: #641010;
       color: #641010;
       transition: 3s;
       cursor: pointer;
    }

    /* === Hero Section === */
    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 2rem;
      background: linear-gradient(135deg, #1b0036, #0a0a0f);
    }
    .hero h1 {
      font-size: 3rem;
      color:   #94fc86;
      margin-bottom: 1rem;
    }
    .hero p { max-width: 600px; }

    /* === Sections === */
    section {
      padding: 4rem 2rem;
      max-width: 1000px;
      margin: auto;
    }
    section h2 {
      color:  #94fc86;
      margin-bottom: 1rem;
      font-size: 2rem;
    }
    section p {
      margin-bottom: 1rem;
    }

    /* === Footer === */
    footer {
      background: #011703;
      padding: 2rem;
      text-align: center;
      font-size: 0.9rem;
      margin-top: 2rem;
      border-top: 1px solid #222;
      color: #72872c;
    }

    /* === Simple Animation === */
    .fade-in {
      animation: fadeIn 2s ease-in;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <header>
    <nav>
      <div class="logo"><img src="symbiotic.png" ></div>
      <ul>
        <li><a href="#about">What is Symbiotic?</a></li>
        <li><a href="#works">How it Works</a></li>
        <li><a href="#community">Community</a></li>
        <li><a href="#resources">Resources</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero fade-in">
    <h1>Symbiotic Protocol</h1>
    <p>The future of restaking and universal security across blockchains. 
       Secure. Scalable. Interoperable.</p>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>What is Symbiotic?</h2>
    <p>Symbiotic Protocol is a universal coordination layer for blockchain ecosystems.
       It extends the concept of restaking, enabling assets to secure multiple networks simultaneously.
       Symbiotic Protocol is a system that lets one staked asset (like ETH) be used across multiple blockchains or 
       applications at the same time. This process is often called restaking, but Symbiotic takes it further by
        allowing something called universal staking.

Here’s how it works technically:<br><br>

1. Staking → Normally, when you stake tokens, they’re locked on one blockchain to secure it.
 You can’t use those same tokens elsewhere.<br><br>


2. Restaking → Symbiotic lets those same tokens be reused (via cryptographic proofs) to secure multiple systems. 
For example, your staked ETH could help secure an oracle network and a rollup chain at the same time.<br><br>


3. Vaults → Symbiotic uses staking vaults as containers that define the rules:<br>
  <ul>
    <li><i>Which assets can be staked?</i></li>
    <li><i>What risks are involved?</i></li>
    <li><i>How rewards are distributed??</i></li>
    <li><i>What penalties (slashing) apply for bad behavior</i></li>
   </ul><br><br>



4. Security Sharing → Instead of each blockchain needing its own pool of staked assets, 
they can all tap into the same shared security base.<br><br>




---

 <h6><b>Think of it like this:</b></h6>

Without Symbiotic → Every app needs its own bodyguard (expensive).

With Symbiotic → One big security team protects multiple apps, and each app pays less.


The “technical magic” is that Symbiotic coordinates these vaults in a way that’s modular and permissionless — 
meaning anyone can build new vaults or connect new systems without needing permission from a central authority.


---

 In short: Symbiotic is building a universal coordination layer where one set of staked assets can secure many
 different blockchains and applications at once, with customizable rules for rewards, risks, and slashing.</p>
  </section>

  <!-- How it Works -->
  <section id="works">
    <h2>How it Works</h2>
    <p>Through staking vaults, users can allocate collateral across chains,
       providing security while unlocking new economic primitives.<br><br>
       Step 1: Deposit Assets

You (a staker) put tokens like ETH, stablecoins, or other assets into a vault on Symbiotic.Step 1: Deposit Assets

You (a staker) put tokens like ETH, stablecoins, or other assets into a vault on Symbiotic.

A vault is basically a smart contract that holds the assets and
 defines the rules (who can join, rewards, penalties, etc.).<br><br>

🛡 Step 2: Validators Join

Validators (the computers that secure blockchains) connect to the vault.

When they use your staked tokens, they are basically saying:
“I’ll keep your assets safe and follow the rules of this vault.”<br><br>

Step 3: Restaking Across Systems

Normally, your ETH might only secure Ethereum.

With Symbiotic, the same ETH can secure multiple things at once, like:

A Layer 2 rollup

An oracle network

A new blockchain project



This works through cryptographic proofs that show your tokens are staked and 
“committed” without having to move them around each time.<br><br>
 Step 4: Rewards + Risks

Since your tokens are working in multiple places, you can earn multiple sets of rewards (like extra yield).

But there are also risks:

If a validator misbehaves on one system, some of your tokens could be “slashed” (burned or taken away).

Each vault defines how much risk you take and how slashing works.<br><br>

Step 5: Modularity

The cool thing is that Symbiotic is modular.

Anyone can create a vault with custom rules (like a Lego block).

Projects can pick which vault to use, what assets to accept, and how security is enforced.<br><br>

</p>
  </section>

  <!-- Community -->
  <section id="community">
    <h2>Community</h2>
    <p>Join the conversation on Discord, contribute on GitHub, 
       and follow Symbiotic on Twitter for the latest updates.</p>
    <ul>
      <li><a href="https://discord.symbiotic.fi/">Discord</a></li>
      <li><a href="https://github.com/symbioticfi">GitHub</a></li>
      <li><a href=" https://x.com/symbioticfi?t=9dvNGe9LLsu6UGzPuz_WeA&s=08">Twitter</a></li>
    </ul>
  </section>

  <!-- Resources -->
  <section id="resources">
    <h2>Resources</h2>
    <p>Learn more about Symbiotic Protocol:</p>
    <ul>
      <li><a href="https://docs.symbiotic.fi/">Documentation</a></li>
      <li><a href="https://blog.symbiotic.fi/">Blog</a></li>
    </ul>
  </section>

  <!-- Footer -->
  <footer>
    <p><i><B>Built with love by the Symbiotic community. Contribution Zone Project.</B></i></p>
  </footer>

</body>
</html>
</body>
</html>
