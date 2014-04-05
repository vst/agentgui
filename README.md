# agentgui

An Editor for X-Machines Markup Language.

This is a quick quide on how to compile, run, install the application
on both Ubuntu and Mac OSX.

## On Ubuntu Linux

    # Get build tools:
    sudo apt-get install qt4-dev-tools libqscintilla2-dev

    # Compile
    qmake build.pro
    make

    # Run
    LD_LIBRARY_PATH=libxmm2/lib/ ./xmme/compilation/agentgui

    # Install
    sudo cp libxmm2/lib/* /usr/lib/
    sudo cp xmme/compilation/agentgui /usr/bin/

### On Mac OSX

    # Get build tools:
    brew install qt4
    brew install qscintilla2

    # Compile
    /usr/local/Cellar/qt/4.8.5/bin/qmake build.pro
    /usr/local/Cellar/qt/4.8.5/bin/macdeployqt xmme/compilation/agentgui.app

    # Run
    open /xmme/compilation/agentgui.app

    # Create a dmg:
    /usr/local/Cellar/qt/4.8.5/bin/macdeployqt xmme/compilation/agentgui.app -dmg
