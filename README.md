# PWA Implementation .Net Core 



#### 1. Install WebEssentials.AspNetCore.PWA 

```
NuGet\Install-Package WebEssentials.AspNetCore.PWA -Version 1.0.65
```



#### 2. Create manifest.json under wwwroot folder

Set ***Copy to Output Directory properties*** to ***Copy Always***

```
// Insert this inside manifest.json
{
  "name": "TestPWA",
  "short_name": "TestPWA",
  "display": "standalone",
  "start_url": "/",
  "icons": [
    {
      "src": "images/icon192x192.png",
      "sizes": "192x192",
      "type": "image/png",
      "purpose": "maskable any"
    },
    {
      "src": "images/icon512x512.png",
      "sizes": "512x512",
      "type": "image/png",
      "purpose": "maskable any"
    }
  ]
}
```

#### 3. Provide an images for PWA Icon 

Place the image under wwwroot folder.  

Under manifes.json, set the src value of icons node where the corresponsing image is located.



