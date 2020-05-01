(function(ext) {
    // Cleanup function when the extension is unloaded
    ext._shutdown = function() {};

    // Status reporting code
    // Use this to report missing hardware, plugin or unsupported browser
    ext._getStatus = function() {
        return {status: 2, msg: 'Ready'};
    };

    // Block and block menu descriptions
    var descriptor = {
        blocks: [
          ['enter','enter key pressed?','key enter pressed?']
        ]
    };
    // Register the extension
    ScratchExtensions.register('Extension', descriptor, ext);
})({});
// Ths is in case our code gets wiped.