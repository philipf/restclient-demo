# REST Client cheat sheet

This repository demonstrates how to use the popular [REST Client extension](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) in VS Code developed by Huachao Mao

## Installation
1. Install the REST Client Extension for Visual Studio code
2. Copy `.vscode/settings.template.json` to `.vscode/settings.json`
3. Update the `local` environment in `settings.json` with your App Registration secrets. This only required for the examples in `05-Authentication.http`
4. Run the examples in the `*.http` files

## Optional installation steps
This repository contains examples that are making request to a locally installed [httpbin](https://httpbin.org/) instance. 
httpbin is a simple web server that echo's HTTP requests back to the client. It is useful for testing purposes.

> **Warning**
> As the examples in `05-Authentication.http` is posting access tokens to httpbin, it is recommended to run httpbin locally.

```powershell
docker run -d --rm -p 8884:80 kennethreitz/httpbin
```

## References
- [REST Client Repository](https://github.com/Huachao/vscode-restclient#environment-variables)
- [REST Client Documentation](https://github.com/Huachao/vscode-restclient#readme)
- [Visual Studio extension by Mads Kirstensen](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.RestClient)