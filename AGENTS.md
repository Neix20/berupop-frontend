# BeruPop Scammer UI Development Guidelines

## File Directory Structure

- Follow modular architecture: `src/{api,app,components,config,hooks,libs}/` with entity-based organization
- Use index.js files for clean exports/imports consolidation in each directory
- Organize API calls by entity (User, Product, Scammer) with separate CRUD operations

## Coding Structure & Style  

- React 18 functional components with Material-UI v6, Redux persistence, and custom hooks
- Use "Bp" prefix for BeruPop components, camelCase variables, path aliases (@api, @components, @config, etc.)
- AWS Amplify + Cognito authentication pattern with environment variable configuration

## Environment Variables

- Use VITE_ prefix for all environment variables (API_URL, LOG_URL, HOST_URL, AWS configs)
- Store constants in `src/config/clsConst.js` and import via destructuring pattern
