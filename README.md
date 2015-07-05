# uv-size-tool

This little tool helps you visualize real world sizes based on the size of an underlying UV map for a three-dimensional model.

![Screenshot][1]


## Usage

* Clone the project and open the index file
* Drag and drop a wavefront object file containing the model and UV information onto the page
* You can see the object dimensions on top of the page for a given UV size
* Change the UV size using the slider or the input field to see the changes for the overal object size
* You can add multiple models to compare their relative sizes

Known limitations:

* Object must contain triangles only! This tool does not support quad faces yet
* .obj file must contain exactly one object (see [example file][4] for details)


## Why?

![Workflow][2]

Using digital three-dimensional models is a good way to create patterns for papercrafting or plush projects. In this process, a three-dimensional model is unwrapped using standard UV-unwrapping algorithms to create a two-dimensional pattern which is then printed and assembled in the real world.

UV coordinates are usually normalized to have a value between 0 and 1. Before printing, this range must be transformed into real-world coordinates (e.g. centimeters). However, performing this step using only the pattern makes it hard to visualize the size of the assembled model. Therefore this tool shows the width, height and depth of the model in relation to the size of the pattern. It also allows displaying multiple models to compare their relative sizes.


## License

[GPL v2][3]


[1]: docs/screenshot.png
[2]: docs/workflow.png
[3]: LICENSE
[4]: example/cube.obj
