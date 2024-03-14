# Commands to run docker 
-  docker build -t react-docker .          -> for image 
-  docker run react-docker                 -> for container
-  docker run -p 5173:5173 react-docker    -> for port forwarding
-  use --host to expose                    -> for vite in package.json        -> "scripts": { "dev": "vite --host", ....
- docker run -p 5173:5173 -v "$(pwd):/app" -v /app/node_modules react-docker  -> For auto updating when changes happens


# To publish your image in Docker hub
- docker login                                     (Logged in automatically if desktop login is done before)
- docker tag react-docker mktintumon/react-docker  (default tag will be latest)
- docker push mktintumon/react-docker
