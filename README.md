# Water Resources

Here's a list of links and references to various pieces of research/games/systems which contain water rendering and could be of interest and inspiration!

If you know of an interesting example of that is missing from this list, please create an issue or pull request!

### Core work

* A classic - Simulating Ocean Water - Tessendorf - has iWave approach for interactive apps: http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.131.5567&rep=rep1&type=pdf
* Also from tessendorf: https://people.cs.clemson.edu/~jtessen/papers_files/Interactive_Water_Surfaces.pdf
* Great thesis about implementing water sim into frostbite: http://www.dice.se/wp-content/uploads/2014/12/water-interaction-ottosson_bjorn.pdf
* Rigorous follow up work to Ottosson: https://gmrv.es/Publications/2016/CMTKPO16/main.pdf
* Water sim on (fixed) quad tree, talks about some of the issues with this: https://pdfs.semanticscholar.org/a3c5/5aeda63895d846c38ae23e921cec7320f584.pdf
* Strugar does multiple overlapping sims: article: http://vertexasylum.com/2010/10/30/gpu-based-water-simulator-thingie/ , video: https://www.youtube.com/watch?time_continue=20&v=jrhjxudnMNg
* GDC course notes from matthias mueller fischer: http://matthias-mueller-fischer.ch/talks/GDC2008.pdf
* Slightly old list of CG water references: http://vterrain.org/Water/
* Mueller - swe + splashes, ripples - nice results: https://pdfs.semanticscholar.org/e97f/38cb774c96aaf1c359d8331695efa3b2c26c.pdf , video: https://www.youtube.com/watch?v=bojdpqi2l_o
* Gomez 2000 - Interactive Simulation of Water Surfaces - Game Programming Gems
* Real-Time Open Water Environments with Interacting Objects - Cords and Staadt. Discusses/justifies multiple sims. Divides collision shapes into particles. - http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.162.2833&rep=rep1&type=pdf
* Hydrax - open source ocean plug-in for OGRE - https://github.com/imperative/CommunityHydrax
* Survey ocean simulation techniques - 2011 - https://arxiv.org/pdf/1109.6494.pdf
* Weta - Synthesizing waves from animated heightfields - 2012 - deals with optimizing a physical ocean surface to match an artist authored shape, numerical issues with tanh(), eliminating overlaps, computing a 3D velocity field: http://cs.au.dk/~bang/publications/NielsenSoderstromBridsonTOG2012.pdf
* Hitman Ocean Technology - they mix a few systems together (thanks for link @ajweeks) https://www.eidosmontreal.com/en/news/hitman-ocean-technology
* Kass - derive / justify wave equation: http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.89.1204&rep=rep1&type=pdf


### Wave Theory

* Great text about water waves of all types: https://topex.ucsd.edu/ps/trujillo_waves.pdf
* Nice chapter on water wave phenomena: http://www.dartmouth.edu/~cushman/books/EFM/chap4.pdf . Shows pressure profile of wind travelling over and obstacle.
* Useful notes on dispersive and non-dispersive waves: http://www-eaps.mit.edu/~rap/courses/12333_notes/dispersion.pdf
* More notes on waves: https://thayer.dartmouth.edu/~d30345d/books/EFM/chap4.pdf
* Dispersive wave equation: https://ccrma.stanford.edu/~jos/pasp/Dispersive_1D_Wave_Equation.html
* Dispersion does not apply to tsunamis: http://www.bu.edu/pasi-tsunami/files/2013/01/daytwo12.pdf
* Longer wavelengths travel faster. For a swell, longest wavelengths arrive first: 
..* https://physics.stackexchange.com/questions/121327/what-determines-the-speed-of-waves-in-water/121330#121330
..* https://en.wikipedia.org/wiki/Wind_wave
* Detailed SWE description from Thuerey: https://pdfs.semanticscholar.org/c902/c4f2c61734cbf4ec7ee8b792ccb01644943d.pdf
* Using SWE for ocean on large scales: http://kestrel.nmt.edu/~raymond/classes/ph332/notes/shallowgov/shallowgov.pdf
* Three stages of how wind generates waves, with refs: https://www.wikiwaves.org/Ocean-Wave_Spectra
* Miles - how energy is transferred from wind to wave: https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/on-the-generation-of-surface-waves-by-shear-flows/40B503619B6D4571BEF3D31CB8925084
* Realistic simulation of waves using wave spectra: https://hal.archives-ouvertes.fr/file/index/docid/307938/filename/frechot_realistic_simulation_of_ocean_surface_using_wave_spectra.pdf
* Nice practical demo about testing different wave breakers: https://youtu.be/3yNoy4H2Z-o
* Useful notes/diagrams on waves: http://hyperphysics.phy-astr.gsu.edu/hbase/Waves/watwav2.html, http://hyperphysics.phy-astr.gsu.edu/hbase/watwav.html#c1
* Nice slides on natural wave phenomena http://www2.ess.ucla.edu/~schauble/EPSS15_Oceanography/LEC13S17_Waves_6perpage.pdf
* Demonstration that Gerstner wave motion is physically possible https://www.tandfonline.com/doi/abs/10.2991/jnmp.2008.15.S2.7

### Wave Simulation

* Mode splitting - surface + volume sim combined: http://www.hilkocords.de/publications/mode_splitting.pdf
* Boat interaction: https://www.youtube.com/watch?v=YK_Za2MY2a0 , paper: http://www.hilkocords.de/publications/open_water.pdf
* Setting up boat interactioin in maya: https://www.youtube.com/watch?v=O-8ow82gQw8 . Touches on issues related to combining heightfield with displacement texture, and the wake lagging behind the object.
* Water Surface Wavelets - Jeschke et al. SIGGRAPH 2018 - http://visualcomputing.ist.ac.at/publications/2018/WSW/ - Interesting rederivation of water motion into a more computationally friendly form. The LOD system in Crest is very competitive with this technique.
* Lecture notes on numerical wave sim, makes use of Courant number directly - https://www.uio.no/studier/emner/matnat/ifi/nedlagte-emner/INF2340/v05/foiler/sim04.pdf
* Insomniac's Water Rendering System for Resistance 2: https://www.gamedevs.org/uploads/insomniac-water.pdf 

### Wave Particles

* Original wave particles work: http://www.cemyuksel.com/research/waveparticles/
* Water Surface Wavelets: http://visualcomputing.ist.ac.at/publications/2018/WSW/

### 3D Simulation

* Bubble sim. Hill spherical vortex - irrotational flow around sphere. http://matthias-mueller-fischer.ch/publications/bubbles.pdf

