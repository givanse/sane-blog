
## Node
    
install [nvm](https://github.com/creationix/nvm)

    curl https://raw.githubusercontent.com/creationix/nvm/v0.24.1/install.sh | bash
    nvm install 0.10
    
## Sails

    npm install -g sails
    npm install -g ember-cli
    npm install -g sane-cli
    
    sane new sane-blog
    cd sane-blog/
    
    # https://github.com/artificialio/sane/issues/141
    cd server/
    npm install --save balderdashy/sails-hook-dev
    
    npm install --save sails-hook-seed
    mkdir -p seeds/development/
    vi seeds/development/PostSeed.js
    cd -
    
    sane up
    
    sane generate resource post title:string body:string
    
    cd client/
