# ⚡ ANGULAR COMPLETE MASTER GUIDE  
## 🚀 Beginner → Advanced → Pro Frontend Framework

---

# 📖 What is Angular?

### English
Angular is a TypeScript-based frontend framework developed by Google for building large-scale single-page applications (SPA).

### বাংলা
Angular হলো Google-এর তৈরি TypeScript-based frontend framework, যা দিয়ে বড় এবং powerful single page application (SPA) তৈরি করা যায়।

---

# 🌟 Why Angular?

- ⚡ Fast SPA Development
- 🧠 TypeScript Support
- 🏗️ Component Based Architecture
- 🌐 REST API Integration
- 🔐 Built-in Security
- 📦 Enterprise Level Applications

---

# 🛠️ INSTALLATION

## Install Angular CLI

```bash
npm install -g @angular/cli
```

---

## Check Version

```bash
ng version
```

---

## Create Project

```bash
ng new my-app
```

---

## Run Project

```bash
cd my-app
ng serve
```

👉 Open:
```
http://localhost:4200
```

---

# 📁 PROJECT STRUCTURE

```
src/
 ├── app/
 │    ├── components/
 │    ├── services/
 │    ├── modules/
 │    ├── app.component.ts
 │    ├── app.module.ts
 ├── assets/
 ├── environments/
```

---

# ⚙️ ANGULAR COMMANDS

## Generate Component

```bash
ng g c home
```

---

## Generate Service

```bash
ng g s api
```

---

## Generate Module

```bash
ng g m auth
```

---

## Build Project

```bash
ng build
```

---

## Production Build

```bash
ng build --configuration production
```

---

# 👋 BASIC COMPONENT

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html'
})
export class AppComponent {
  title = 'Angular App';
}
```

---

# 🌐 DATA BINDING

## Interpolation

```html
{{ title }}
```

---

## Property Binding

```html
<img [src]="imageUrl">
```

---

## Event Binding

```html
<button (click)="clickMe()">Click</button>
```

---

## Two Way Binding

```html
<input [(ngModel)]="name">
```

---

# 📦 DIRECTIVES

## ngIf

```html
<p *ngIf="isActive">Active</p>
```

---

## ngFor

```html
<li *ngFor="let item of items">{{item}}</li>
```

---

# 🌐 API CALL (HTTP)

## Import HttpClient

```ts
import { HttpClient } from '@angular/common/http';
```

---

## Service Example

```ts
constructor(private http: HttpClient){}

getUsers(){
  return this.http.get("https://api.example.com/users");
}
```

---

# 🔐 ROUTING

## Routes Setup

```ts
const routes: Routes = [
  { path: '', component: HomeComponent },
  { path:
