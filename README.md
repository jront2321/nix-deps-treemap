# Dependency graph treemap visualization! :)

![image](https://github.com/user-attachments/assets/0d931c01-df08-405a-b7ef-5485df7d2901)

## Instructions

1. Clone repo
2. Run the bash script on a derivation, eg `./deps.sh /nix/store/z49g31nnd5hkf2di6gp693mlsp23xdgh-python3.10-remarks-0.3.10`
3. Open the html file
4. Open the generated JSON file

### Get derivation path for a flake build

If you have a flake that builds a package, you can get the path with `nix build .#my-derivation --no-link --print-out-paths`

### What the heck is a treemap?

> Introduced by Ben Shneiderman in 1991, a treemap recursively subdivides area into rectangles according to each node’s associated value. D3’s treemap implementation supports an extensible tiling method: the default squarified method seeks to generate rectangles with a golden aspect ratio; this offers better readability and size estimation than slice-and-dice, which simply alternates between horizontal and vertical subdivision by depth.

[source](https://d3js.org/d3-hierarchy/treemap)
