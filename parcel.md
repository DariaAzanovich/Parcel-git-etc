# Parcel 

1. Install Node JS 
    + ```node --version```

2. Install npm
    + ```npm -v```

3. Create package.json
    + ```npm init -y``` 

4. Install Parcel
   +  ```npm install parcel-bundler --save-dev```

5. Create folder 
    + ```src```

6. Go to **package.json** --> **scripts**
    + create script: ```"dev": "parcel ./src/index.html"```

7. Open terminal
    + ```npm run dev````

8. Click at 
    + http://localhost:1234 

9. Create build 
    + create script: ``` "build": "parcel build ./src/index.html --no-source-maps"```

10. Build project
    + ```npm run build```

### The end