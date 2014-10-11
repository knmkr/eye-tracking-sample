# Eye Tracking Mouse

Control mouse curser with eyes


## Getting Started

Install OpenCV via Homebrew

    $ brew tap homebrew/science
    $ brew install opencv

Prepare haarcascades files

    $ cd /path/to/this/repository
    $ brew list opencv| grep share\/OpenCV\/haarcascades| xargs -Ix ln -s x .

Compile

    $ g++ -o main eye-tracking.cpp `pkg-config --cflags opencv` `pkg-config --libs opencv`
