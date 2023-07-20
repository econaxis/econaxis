+++
title="Henry Nguyen's Portfolio"
template="page.html"

+++

- 👋 Hi, I’m Henry Nguyen
- 📚 I'm a computer science student at the University of Waterloo
- 👀 I’m interested in databases, graphics, public transit, and maps
- 🏢 I'm currently looking for 2024 internships!
- 📫 How to reach me: email h99nguye at uwaterloo.ca


# Here are some of my projects:

<img src="/image.png" width="500px" class="first-image" />

- [**Interactive travel time map**](https://map.henryn.xyz) - An interactive travel time map that shows you how far you can go using public transit. 


<img src="/renderer.gif" width="500px">

- [**3d renderer**](https://3d-renderer.netlify.app) - An image buffer, triangle rasterizer, 3d renderer from scratch. Includes shadows, highlights, ambient lighting, and various performance optimizations. Compiled to WASM.

![video](/ezgif-2-23ab435b8008.gif)

- [**Transit map**](https://github.com/econaxis/transit) - *([longer video here](https://youtu.be/sEx_jOtT0IM))* - 
Map visualization of 1000+ Toronto buses travelling in real-time. Uses WebGL and some performance optimizations to do 60FPS rendering of that many buses.
For a better video than the GIF, I have a [Youtube video](https://youtu.be/sEx_jOtT0IM)


<img src="/search.mp4" width="800px">

 - [**Full-text search engine**](https://github.com/econaxis/search) - A full-text search engine (like Elasticsearch). Demo includes near-instant textual search of all English Wikibooks articles. Uses *db1* as the underlying storage engine

 - [**Coroutines and garbage collector in C**](https://github.com/econaxis/coroutines) - 
Userspace context switching, multitasking without threads, or stackful, preemptive multitasking. Implemented with some small inline assembly and register manipulation. Made a fair task scheduler based off the Linux CFS scheduling algorithm.
Mark-and-sweep garbage collector in C. Implemented using `pycparser` to modify C code, and custom stack frames to find GC roots. 



 - [**Custom DNS Nameserver**](https://github.com/econaxis/dns) - Authorative DNS nameserver (based off RFC 1034/1035) from scratch.

 - [**JSON database**](https://github.com/econaxis/database) - A fully transactional, ACID database that can store infinite depth JSON objects. Primitive support for replicated transactions using gRPC. 

 - [**db1**](https://github.com/econaxis/db1) - A second iteration attempt to make a database. A simpler key-value database with static schema, fixed-size tuples, and columnar compression. Built for use by my search engine




 - [**Automatic ATC with A\* pathfinding**](https://github.com/econaxis/atc/) - Routes incoming airplanes to one of two runways while avoiding collisions. Done for a coding assignment. 

 - [**Beeeeeep**](https://github.com/econaxis/beeeeeep) - Experiments with audio processing and modulation to send and receive binary data over audio at 1kbps. 

 - [**Bridge Static Analysis**](https://github.com/econaxis/struss) - Solves forces on bridges and uses random search to minimize cost of bridge.



<img src="/README_image.jpg" width="500px">

 - [**Interactive ontology visualization**](https://github.com/climateMind/climatemind-ontology-visualization) -
Interactive knowledge graph visualization built using Cytoscape.JS and Python backend. Generated Docker images for easy deployment. 


 - [**Othello game with AI**](https://github.com/econaxis/othello) -
An othello game made for my university class. Implemented a minimax AI algorithm with culling. 

# Work Related Projects

- *Transify* - I forked the open source routing engine Graphhopper (Java) for more accurate isochrones on geometries with sparse intersections and batch shortest-path-tree calculations. Decreased runtime of analyzing Brampton transit accessibility from 32 seconds to 2 seconds. This feature is used by transit planners to determine which areas a bus route serves and calculate demographics such as how many jobs or homes are on the route.

- *Transify* - I created a realtime map of bus vehicle locations using Node.JS and React, with automated builds and deployments to GKE. This is useful for transit agencies to see at a glance which buses are delayed and need help along a route.

- *Dropbase* - I built a Pandas-compatible Excel parser optimized for chunked, larger-than-memory reading based off the open source library Calamine. I then built a Python wrapper around the native Rust library, setup automated Github Actions builds, and did extensive testing to make sure the new parser was compliant with Pandas.

- *Dropbase* - When profiling, I found that `dateutil` was taking up 99% of our task runtimes. [This](https://www.kaggle.com/code/kuldeepnpatel/to-datetime-is-too-slow-on-large-dataset) [is](https://stackoverflow.com/questions/14163399/convert-list-of-datestrings-to-datetime-very-slow-with-python-strptime) [a very](https://stackoverflow.com/questions/13468126/a-faster-strptime) [common](https://stackoverflow.com/questions/52480839/slow-pd-to-datetime) [problem](https://github.com/pandas-dev/pandas/issues/9714). Since Dropbase tries to accept all CSVs and tries to parse them into a structured format, I created an optimize datetime parser for Rust that handles all types of formats with/without timezones. 


# Resume

If you're interested, [my resume is also available](/resume.pdf).

<!---
econaxis/econaxis is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
