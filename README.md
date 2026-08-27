# Source Choreo Objects

This repo contains the **.vpc** setup for compiling the **choreoobjects.lib** for Source Engine. This is valid for all versions of Source Engine.

## Integrating

Add the following to **vpc_scripts/projects.vgc**:
```
$Project "choreoobjects"
{
	"choreoobjects\choreoobjects.vpc"
}
```
Then, in **vpc_scripts/groups.vgc**, add `"choreoobjects"` to the group of your choice.

## Notes

This `.vpc` was reverse-engineered by inspecting **choreoobjects.lib** in IDA and cross-referencing its exported symbols against the source files in the Source SDK.
