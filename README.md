--GPC Repo--

To the run agruments, put the output in a /bin/ directory currently ignored by .gitignore: 
Example of tasks.json on VSCode (MacOS)
{
    "tasks": [
        {
            "type": "cppbuild",
            "label": "C/C++: g++ build active file",
            "command": "/usr/bin/g++",
            "args": [
                "-g",
                "${file}",
                "-o",
                "${fileDirname}/bin/${fileBasenameNoExtension}",
                "-framework",
                "Cocoa",
                "-framework",
                "OpenGL",
                "-framework",
                "glut",
            ],
            "options": {
                "cwd": "${fileDirname}"
            },
            "problemMatcher": [
                "$gcc"
            ],
            "group": {
                "kind": "build",
                "isDefault": true
            },
            "detail": "Task generated by Debugger."
        }
    ],
    "version": "2.0.0"
}

