# Standalone Class Demonstration

This folder is a browser-only version of the warranty claim-readiness prototype. It uses synthetic data and local JavaScript checks; it does not connect to FastAPI, SQLite, Hyundai systems, or any external service.

## Test locally

Open `demo/index.html` directly in a browser, or run:

```bash
python3 -m http.server 8080 --directory demo
```

Then open <http://127.0.0.1:8080>.

## Share with a professor using Vercel

### Dashboard method

1. Create or sign in to a Vercel account at <https://vercel.com>.
2. Create a new project from a Git repository containing this `demo` folder.
3. Set the project root directory to `demo`.
4. Leave the framework preset as **Other** and leave the build command blank.
5. Deploy the project.
6. Copy the generated `vercel.app` URL into Canvas.

### CLI method

After installing Node.js and the Vercel CLI, run from the repository root:

```bash
npx vercel demo
```

Follow the prompts, then copy the deployment URL printed by Vercel. To create a production deployment, use:

```bash
npx vercel demo --prod
```

The resulting HTTPS URL can be opened from another device without running Python. The demo remains browser-only and uses synthetic data.
