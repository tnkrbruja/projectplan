```.
├── my-project/
├── ├── .github/                     # CI/CD workflows
├── ├── apps/                        # Deployable applications
├── │   ├── web/                     # 🌐 NEXT.JS FRONTEND (Deploys to Vercel)
├── │   │   ├── app/                 # App Router (layout.js, page.js)
│   │   │   └── inventory-form/
│   │   |        └── page.js          # <form> UI with Tailwind styling
├── │   │   ├── components/          # UI Components
├── │   │   ├── public/              # Static assets
├── │   │   ├── next.config.js       
├── │   │   ├── tailwind.config.js   # Tailwind Configuration
├── │   │   └── package.json
├── │   │
├── │   └── server/                  # 🖥️ EXPRESS.JS BACKEND (Deploys to Render/Fly.io/AWS)
├── │       ├── src/
├── │       │   ├── controllers/
│           │     └── formController.js # Extracts payloads & orchestrates logic
    │           └── routes/
│                   └── api.js           # POST /api/forms/submit
├── │       │   ├── middleware/
├── │       │   ├── services/
├── │       │   │   └── notion.js    # Notion SDK implementation
├── │       │   └── index.js         # Express Entry point
├── │       └── package.json
├── │
├── ├── middleware/                  # ⚙️ GOOGLE APP SCRIPT
├── │   ├── src/
├── │   │   └── Code.js              # GAS Logic (Webhooks, Form Handlers, etc.)
├── │   ├── appsscript.json          # GAS Manifest
├── │   └── clasp.json               # Google Clasp config for CLI pushing
├── │
├── ├── packages/                    # Shared configurations (Optional)
├── │   └── tsconfig/
├── │
├── ├── package.json                 # Root package.json defining workspaces
└── └── pnpm-workspace.yaml          # Workspace config (if using pnpm)
```


