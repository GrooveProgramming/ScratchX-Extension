(function(ext) {

    ext._shutdown = function() {};



    ext._getStatus = function() {
        return {status: 2, msg: 'Ready'};
    };


    var descriptor = {
        blocks: [
            ['b','loud?','loud']
        ]
    };


    ScratchExtensions.register('Extension', descriptor, ext);
})({});

// Ths is in case our code gets wiped.
