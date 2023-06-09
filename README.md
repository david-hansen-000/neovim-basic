# neovim-basic

building and running neovim on most platforms

clone neovim from github

git clone https://github.com/neovim/neovim.git

cd neovim

(optional checkout the latest stable version)

git tag

#will load all the available tags for the repository
#hit space bar to keep scrolling to the bottom
#the last one is the latest

v0.9.1 
#is latest at time of this writing

git checkout v0.9.1
#change "v0.9.1" to the latest

mkdir .deps

mkdir build

cd .deps

cmake -G Ninja -DCMAKE_BUILD_TYPE=Release ../cmake.deps/

ninja

cd ..

cd build

cmake -G Ninja -DCMAKE_BUILD_TYPE=Release ..

ninja

sudo ninja install
#or gsudo for windows or will need to run ninja install in the build directory from an elevated permission ie superuser or admin account


