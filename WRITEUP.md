# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

- In terms of costs, VMs are more expensive but they offer full control over the server (which would be very important if our solution required tight control over the operating system, for example); although this amount of control comes with a downside: scaling depends on the developer. An App Service, in the other hand, limits the control the developer has over the host server but has high-availability and supports autoscaling (and is also worth remembering that the App Service have both memory and computing limitations)
- For this partiuclar app, an App Service would suffice because we don't need a lot of control over the host server and the language used to make the app is supported (Python). However, this decision might need to be revised if for instance we expect the amount of needed memory to surpass the 14GB memory threshold or the 4 vCPU cores per instance in terms of computing power (in that case, we would need a VM with more memory and/or computing resources).
