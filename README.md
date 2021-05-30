# Wavefront OBJ mesh exporter

Minimal [Wavefront OBJ](https://en.wikipedia.org/wiki/Wavefront_.obj_file) mesh geometry exporter script. Only supports meshes with indexed vertex data and does not export materials.

## Usage

Copy the `objexport.gd` -file to your project directory and use it for example like this:

	var mesh = SphereMesh.new()

	var obj_export = load("res://objexport.gd").new()
	obj_export.save_mesh_to_obj(mesh, "output.obj", "mymesh")

The first argument to the function is the mesh resource to be saved, second is the output file name and third is the name for the object inside the exported file.

## License

MIT license.

This was initially made for dumping procedurally generated level mesh to file for debugging in [Polychoron](https://www.fractilegames.com/polychoron/) game project.
