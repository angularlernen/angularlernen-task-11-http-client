HttpClient
==========

### Introduction

Great, we have some solid services now! Let's work with a real data source.

### Preparation

If you haven't the API up and running, start it: `json-server --watch microevents.json`

### Task

Remove the hardcoded data arrays in the `api` modules _injectables_, thus _EventResource_ and _ProfileResource_.

Use the `HttpClient` injectable out of the `HttpClientModule` instead.

### HOWTOs

#### api.module.ts

```ts
import { HttpClientModule } from "@angular/common/http";
```

```ts
@NgModule({
  imports: [
    // ...
    HttpClientModule
  ],
}) // ...
```

#### event.resource.ts - findAll

`import { HttpClient } from "@angular/common/http";`

`http://localhost:3000/events`

#### profile.resource.ts - findAll

`import { HttpClient } from "@angular/common/http";`

`http://localhost:3000/profiles`
