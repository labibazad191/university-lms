# UniversityLms

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 21.1.4.

node -v
npm -v

## Install Angular CLI globally:

npm install -g @angular/cli


## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

## STEP 2: Create Angular Project

ng new university-lms

cd university-lms

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

## STEP 3: Create Project Structure (Modules)

ng g module modules/auth --routing
ng g module modules/admin --routing
ng g module modules/student --routing
ng g module modules/teacher --routing
ng g module shared

## Building

## STEP 4: Create Components
Auth Components
ng g c modules/auth/login
ng g c modules/auth/register

## Admin Components

ng g c modules/admin/dashboard
ng g c modules/admin/manage-users
ng g c modules/admin/manage-courses


## Student Components
ng g c modules/student/dashboard
ng g c modules/student/my-courses
ng g c modules/student/assignments


## Teacher Components
ng g c modules/teacher/dashboard
ng g c modules/teacher/create-course
ng g c modules/teacher/upload-material



## STEP 5: Create Core Services

## Create API service:

ng g service core/services/api

## Create auth service:

ng g service core/services/auth

## Create course service:

ng g service core/services/course




## STEP 6: Setup Routing (Main app-routing.module.ts)
const routes: Routes = [
  { path: '', redirectTo: 'auth/login', pathMatch: 'full' },

  {
    path: 'auth',
    loadChildren: () =>
      import('./modules/auth/auth.module').then(m => m.AuthModule)
  },
  {
    path: 'admin',
    loadChildren: () =>
      import('./modules/admin/admin.module').then(m => m.AdminModule)
  },
  {
    path: 'student',
    loadChildren: () =>
      import('./modules/student/student.module').then(m => m.StudentModule)
  },
  {
    path: 'teacher',
    loadChildren: () =>
      import('./modules/teacher/teacher.module').then(m => m.TeacherModule)
  }
];



## STEP 7: Add Angular Material (Optional but Recommended)

ng add @angular/material

ng build --configuration production


cd university-lms


npm install -D tailwindcss postcss autoprefixer

npx tailwindcss init

tailwind.config.js

npm install -D tailwindcss @tailwindcss/postcss postcss autoprefixer



## Github 


git init
git remote add origin https://github.com/labibazad191/university-lms.git
git remote set-url origin https://github.com/labibazad191/university-lms.git
git add .
git commit -m "Initial commit - University LMS Angular Project"
git branch -M main
git push -u origin main
git add .
git commit -m "Update LMS project"
git push origin main
git pull origin main --allow-unrelated-histories
git push -u origin main
git push -u origin main --force








## Create postcss.config.js (Manual)

In project root (university-lms/) create:

postcss.config.js
