# Asians Group Console Portal – Playwright Automation Framework

This is an automated testing framework built using **Playwright** to validate key functionality in the **Asians Group Console Portal**, specifically focusing on cache strategy validation and login functionality.

## 🧪 Test Coverage

The framework includes the following test modules:

1. **Login Test**  
   Validates successful and unsuccessful login scenarios.  
   - Command:  
     ```bash
     npx playwright test login.spec.ts
     ```

2. **Cache Modes Test**  
   Verifies proper application and persistence of different cache modes like `public`, `private`, `no-store`, etc.  
   - Command:  
     ```bash
     npx playwright test cachemodes.spec.ts
     ```

3. **Cache TTL Test**  
   Validates Time-To-Live (TTL) settings in cache configurations, including both positive and negative scenarios.  
   - Command:  
     ```bash
     npx playwright test cacheTTL.spec.ts
     ```

4. **Purge Settings Test**  
   Tests cache purge functionality (manual and automated) and ensures frontend reflects the updates properly.  
   - Command:  
     ```bash
     npx playwright test purgeSettings.spec.ts
     ```

---

## 📁 Project Structure

├── tests/
│ ├── login.spec.ts
│ ├── cachemodes.spec.ts
│ ├── cacheTTL.spec.ts
│ └── purgeSettings.spec.ts
├── helpers/
│ ├── credentials.ts
│ └── cacheSettings.ts
├── playwright.config.ts
├── README.md
└── package.json
