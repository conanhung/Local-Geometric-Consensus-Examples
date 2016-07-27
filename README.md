# Local-Geometric-Consensus-Examples

## Installation (Linux Only)

### Prerequisites (Unbuntu)
1. Install cmake
sudo apt-get install cmake

2. Install OpenCV (3.1.0)
http://opencv.org/downloads.html

3. Install PCL
sudo add-apt-repository ppa:v-launchpad-jochen-sprickerhof-de/pcl
sudo apt-get update
sudo apt-get install libpcl-all

4. Install OpenSceneGraph (3.4.0)
http://www.openscenegraph.org/index.php/download-section/stable-releases

5. Download LGC binary

### Complie (Unbuntu)
run script "compileAll.sh"

## Run

### Download models and pre-record videos
1. Download models, extract it and put files inside "models" folder:
https://dl.dropboxusercontent.com/u/274381971/GItLGC/models.zip

2. Download videos, extract it and put files inside "videos" folder:
https://dl.dropboxusercontent.com/u/274381971/GItLGC/videos.zip

### Run examples 
1. cd into "examples" sub-directory
2. run examples:
a) To track a point set:
./build/opencvexample -v ../videos/example.mov -r ../models/A4Pattern.txt -w 1920 -h 1080
b) To augment a point set with a cow:
./build/osgexample ../models/osgexample.xml

### Run applications
1. cd into "applications" sub-directory
2. run applications:
a) To click and track 2D planar objects (support multi-models):
./build/textureTracking -v ../videos/diverseTargets.mpg
b) To augment different engineering draws (support multi-models):
./build/augmentingDrawings ../models/demo.xml

## Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History
9 June 2016: First commit
