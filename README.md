<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0F172A,50:1E3A8A,100:0891B2&text=SynKode&fontSize=76&fontColor=FFFFFF&fontAlignY=34&desc=by%20NexaCore%20Co.&descSize=20&descAlignY=54&animation=fadeIn" width="100%" alt="SynKode by NexaCore Co." />

<a href="https://github.com/crmapp28-nexa">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1200&color=0891B2&center=true&vCenter=true&width=620&lines=Offline-first+desktop+software+for+real+businesses;Native+Windows+apps+built+with+Rust+%2B+React;Point+of+sale+%C2%B7+Inventory+%C2%B7+Warranty+%C2%B7+Reporting;English+%26+Arabic%2C+right-to-left+aware" alt="Offline-first desktop software for real businesses" />
</a>

<br/>

<img src="https://img.shields.io/badge/Tauri-2.x-24C8DB?style=for-the-badge&logo=tauri&logoColor=white" alt="Tauri 2" />
<img src="https://img.shields.io/badge/Rust-Backend-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust backend" />
<img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 19" />
<img src="https://img.shields.io/badge/TypeScript-Strict-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/PostgreSQL-SeaORM-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL with SeaORM" />

<br/><br/>

<img src="https://img.shields.io/badge/Platform-Windows%20Desktop-0078D4?style=flat-square&logo=windowsterminal&logoColor=white" alt="Windows desktop" />
<img src="https://img.shields.io/badge/Runs-100%25%20Offline-16A34A?style=flat-square" alt="Runs fully offline" />
<img src="https://img.shields.io/badge/i18n-English%20%2F%20%D8%A7%D9%84%D8%B9%D8%B1%D8%A8%D9%8A%D8%A9-7C3AED?style=flat-square" alt="English and Arabic" />
<img src="https://img.shields.io/badge/Delivery-NSIS%20Installer%20%2B%20Auto--update-EA580C?style=flat-square" alt="NSIS installer with auto-update" />

</div>

<br/>

---

## ◆ What we build

**SynKode by NexaCore Co.** builds native desktop business software that does not need the cloud to work.

Every product ships as a single Windows installer, keeps its data in a local PostgreSQL database, and runs at full speed with the network unplugged. The interface is React. The engine underneath is Rust. Nothing between them is a browser tab pretending to be an app.

<table>
<tr>
<td width="25%" align="center"><b>Native, not wrapped</b><br/><sub>Rust core over Tauri 2, a few megabytes rather than a few hundred</sub></td>
<td width="25%" align="center"><b>Your data stays yours</b><br/><sub>Local PostgreSQL, no telemetry, no vendor lock</sub></td>
<td width="25%" align="center"><b>Bilingual by design</b><br/><sub>English and Arabic with true right-to-left layout</sub></td>
<td width="25%" align="center"><b>Built to be audited</b><br/><sub>Role-based access, session expiry, activity trails</sub></td>
</tr>
</table>

<br/>

---

## ◆ Products

<table>
<tr>
<td width="50%" valign="top">

### 🧩 Synkode CRM

**Complete CRM and point of sale for retail and wholesale.**

Sales, inventory, purchasing and accounting in one binary. Warehouse-aware checkout with barcode entry, printable receipts, and a built-in calculator at the till.

`Point of sale` `Invoicing` `Quotations` `Sale orders`
`Stock transfers` `Purchase bills` `Cash registers`
`Profit and loss` `PDF and Excel export` `Dual currency`

<a href="https://github.com/crmapp28-nexa/NexaCore-CRM-Setup/releases">
  <img src="https://img.shields.io/badge/Download%20Installer-0F172A?style=for-the-badge&logo=windows&logoColor=white" alt="Download the installer" />
</a>

</td>
<td width="50%" valign="top">

### 🛡️ ZTC Care & Warranty

**Customer care and warranty operations, end to end.**

Warranty claims from intake to delivery, with the parts inventory, payments and maintenance centers that surround them.

`Warranty tracking` `Order pipeline` `Parts inventory`
`Customer payments` `Maintenance centers` `Warehouses`
`Barcode scanning` `Activity log` `Auto-update`

<a href="https://github.com/crmapp28-nexa/ZTC-CARE-WARRANTY-Releases/releases">
  <img src="https://img.shields.io/badge/Latest%20Release-0F172A?style=for-the-badge&logo=github&logoColor=white" alt="Latest release" />
</a>

</td>
</tr>
</table>

<br/>

---

## ◆ How it fits together

```mermaid
flowchart LR
    subgraph shell["Desktop application · single installer"]
        ui["React 19 · TypeScript<br/>shadcn/ui · Tailwind"]
        core["Rust core<br/>Tauri 2 runtime"]
    end
    db[("PostgreSQL<br/>local instance")]

    ui <-->|"typed IPC commands"| core
    core <-->|"SeaORM · versioned migrations"| db

    classDef front fill:#0891B2,stroke:#0E7490,color:#FFFFFF
    classDef back fill:#1E3A8A,stroke:#1E40AF,color:#FFFFFF
    classDef store fill:#0F172A,stroke:#334155,color:#FFFFFF
    class ui front
    class core back
    class db store
```

<br/>

---

## ◆ The stack

<div align="center">

<img src="https://skillicons.dev/icons?i=rust,react,ts,vite,tailwind,postgres,github,vscode&theme=dark&perline=8" alt="Rust, React, TypeScript, Vite, Tailwind, PostgreSQL, GitHub, VS Code" />

</div>

<table>
<tr><td><b>Interface</b></td><td>React 19 · TypeScript · Vite · Tailwind CSS · shadcn/ui · Radix · Recharts · TanStack Table</td></tr>
<tr><td><b>Core</b></td><td>Rust · Tauri 2 · typed command bridge · background services</td></tr>
<tr><td><b>Data</b></td><td>PostgreSQL · SeaORM · a standalone migration crate with versioned, reversible schema</td></tr>
<tr><td><b>Delivery</b></td><td>NSIS installer · built-in updater · GitHub Actions release pipeline</td></tr>
</table>

<br/>

---

## ◆ Activity

<div align="center">

<img height="175" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=crmapp28-nexa&theme=github_dark" alt="Contribution statistics" />
<img height="175" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=crmapp28-nexa&theme=github_dark" alt="Most used languages" />

<br/>

<sub>Most of what we build lives in private repositories, so these counters show only a slice of the work.</sub>

</div>

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=120&color=0:0891B2,50:1E3A8A,100:0F172A" width="100%" alt="" />

</div>
