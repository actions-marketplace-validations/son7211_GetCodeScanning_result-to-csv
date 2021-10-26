# GetCodeScanning

This is simple GitHub Action which gets GitHub Advanced Security - Code Scanning results to JSON. 

- Require `GITHUB_TOKEN` which is automatically generated
- `GITHUB_TOKEN` should have `read` permission for `security`
- This action generate `result.csv` file
- Use [GitHub Upload Action](https://github.com/actions/upload-artifact) to upload the `result.csv` file 

Usage:

 ``` 
  uses : son7211/GetCodeScanning@main
  with :
    github_token: ${{ secrets.GITHUB_TOKEN }}
 ```
