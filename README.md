# Instructions to reproduce

Install dependencies:
```
npm install
```

Start Tailwind CLI build process with minification:
```
npx tailwindcss -i tailwind.css -o tailwind.build.css --watch --minify
```

Start server:
```
http-server
```

Visit `http://127.0.0.1:8081` in Chrome and Safari and you'll see that the styling is broken in Safari. Now, restart Tailwind CLI WITHOUT minification:
```
npx tailwindcss -i tailwind.css -o tailwind.build.css --watch
```

Empty your Safari browser cache and reload the page you'll see that the styling is now working.
