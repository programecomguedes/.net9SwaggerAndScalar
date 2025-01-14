# .NET9 Swagger and Scalar
An example of a .NET 9 project with Swagger and Scalar configured.

## Swagger
- Library: Swashbuckle.AspNetCore.SwaggerUI
```csharp
app.UseSwaggerUI(options => options.SwaggerEndpoint("/openapi/v1.json", "Swagger and Scalar Example"));
```

## Scalar.AspNetCore
- Library: Swashbuckle.AspNetCore.SwaggerUI

```csharp
app.MapScalarApiReference();
```

To working with Docker:
```csharp
app.MapScalarApiReference(options => options.Servers = []);
```

## Enable Swagger and Scalar with Docker
```docker
ENV ASPNETCORE_ENVIRONMENT=Development
```
