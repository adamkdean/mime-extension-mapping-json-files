# mime-extension-mapping-json-files
General purpose mime/extension mapping data in JSON format

## How could you use this?

    var mime2ext = {
        "x-world/x-3dmf":".qd3d",
        "application/octet-stream":".zoo",
        // etc
        "multipart/x-zip":".zip",
        "text/x-script.zsh":".zsh"
    };
    
    var ext = mime2ext["image/pjpeg"];
    
Or

    var ext2mime = {
        ".3dm": "x-world/x-3dmf",
	    ".3dmf": "x-world/x-3dmf",
        // ...
        ".zoo": "application/octet-stream",
	    ".zsh": "text/x-script.zsh"
    };
    
    var mime = ext2mime[".jpg"];
    
