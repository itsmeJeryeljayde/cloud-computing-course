
## 1. Cloud Services I Use

Every day I rely on several cloud-based services without always thinking about the infrastructure behind them:

- **Google Drive** – for storing, syncing, and sharing documents and files
- **Netflix** – for streaming video content on demand
- **GCash** – for mobile payments, transfers, and digital wallet services
- **Messenger** – for real-time messaging and calls

## 2. Identifying the Service and Deployment Models

**Google Drive** is a **SaaS (Software as a Service)** application — I use the finished software through a browser or app without managing any servers or storage infrastructure myself. It runs on a **Public** deployment model, since Google owns and operates the infrastructure and offers it to any user who signs up.

**Netflix** is also **SaaS**, since I only interact with a ready-to-use streaming interface. Behind the scenes, Netflix actually runs much of its infrastructure on Amazon Web Services (an **IaaS/PaaS** layer), but from my perspective as an end user, it is pure SaaS. It follows a **Public** deployment model as well, since anyone with a subscription can access it over the internet.

**GCash** is best classified as **SaaS**, since I use a finished mobile application to send money, pay bills, and check balances. Because it handles sensitive financial data and must comply with banking regulations, it likely runs on a **Hybrid** deployment model — a mix of public cloud infrastructure for scalability and private, tightly controlled servers for handling regulated financial transactions.

**Messenger** is a **SaaS** communication tool, also on a **Public** deployment model, since it's available to any user with a Facebook account.

## 3. Git & GitHub for Cloud Projects

Version control is critical when working with cloud infrastructure because cloud environments are often shared among multiple team members who can each make changes to configuration files, scripts, or deployment code at the same time. Without version control, one person's changes could silently overwrite another's, or a misconfigured file could get deployed to a live cloud environment with no easy way to identify what changed or revert it.

GitHub helps teams collaborate by allowing multiple people to work on separate branches, propose changes through pull requests, and review each other's code before merging it into the main branch. This peer review process catches errors — such as an incorrect cloud resource configuration — before they affect production systems. GitHub also maintains a complete history of every change, including who made it and why, which makes it possible to trace bugs back to their source or roll back to a previous stable state instantly. For cloud infrastructure specifically, this is often paired with practices like Infrastructure as Code, where the entire cloud setup is defined in version-controlled files, making deployments repeatable, auditable, and far less error-prone than manual configuration.
