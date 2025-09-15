# ss-api-http-client
> [auto-generated from ss-api](https://github.com/souzaramon/ss-api)

## Installation

This package is hosted on **GitHub Packages**, which requires authentication via a personal access token (PAT).

1. **Generate a GitHub Personal Access Token (PAT)**

   - Go to [GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate new token](https://github.com/settings/tokens)  
   - Select **`read:packages`** scope.  
   - Copy the token, you’ll need it in the next step.

2. **Set an environment variable with your token**

    On macOS / Linux:  
    ```bash
      export GITHUB_TOKEN=your_personal_access_token
    ```
    
    On Windows (PowerShell):
    
    ```sh
    setx GITHUB_TOKEN "your_personal_access_token"
    ```

3. Create or update your .npmrc file

    Add the following lines to your project .npmrc (or global ~/.npmrc):
    
    ```
    @souzaramon:registry=https://npm.pkg.github.com/
    //npm.pkg.github.com/:_authToken=${GITHUB_TOKEN}
    ```

4. Install the package
    
    ```sh
    npm install @souzaramon/ss-api-http-client
    ```
