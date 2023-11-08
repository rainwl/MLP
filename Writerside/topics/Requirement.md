# Requirement

## Web

| Issue                                          | Description                                                | Remark       | Status |
|------------------------------------------------|------------------------------------------------------------|--------------|--------|
| [#5](https://github.com/rainwl/MLP/issues/5)   | No more than three level directory web page implementation | Already have | TODO   |
| [#15](https://github.com/rainwl/MLP/issues/15) | Provide user login access portal                           | Already have | TODO   |
| [#16](https://github.com/rainwl/MLP/issues/16) | Different users give different permissions                 | ..           | TODO   |
| [#17](https://github.com/rainwl/MLP/issues/17) | Preview window for model                                   | ..           | TODO   |

## Support

| Issue                                          | Description                                                        | Remark                                      | Status |
|------------------------------------------------|--------------------------------------------------------------------|---------------------------------------------|--------|
| [#6](https://github.com/rainwl/MLP/issues/6)   | Supports mainstream 3D model formats                               | Already support fbx、ply、off、obj、3ds、x3d、stl | TODO   |
| [#14](https://github.com/rainwl/MLP/issues/14) | Export the model according to the specified format                 | Already support                             | TODO   |
| [#21](https://github.com/rainwl/MLP/issues/21) | Generate model display links, and provide third-party software     | ..                                          | TODO   |
| [#22](https://github.com/rainwl/MLP/issues/22) | Create a display window in the PPT to achieve the display function | ..                                          | TODO   |

## Retrieval

<procedure title="Current system workflow" id="flow">
    <step>
        <p>The library requires 3D models and their corresponding multiple views</p>
    </step>
    <step>
        <p>The corresponding features of each model are obtained and saved according to multiple views</p>
    </step>
    <step>
        <p>Later, if the user uses the retrieval function </p>
    </step>
    <step>
        <p>The feature is extracted directly from the image input by the user </p>
    </step>
    <step>
        <p>and the Euclidean distance between it and all the features saved before is calculated to find the most similar one </p>
    </step>
</procedure>

| Issue                                          | Description             | Remark                 | Status |
|------------------------------------------------|-------------------------|------------------------|--------|
| [#7](https://github.com/rainwl/MLP/issues/7)   | Retrieval function      | Already have work flow | TODO   |
| [#8](https://github.com/rainwl/MLP/issues/8)   | Retrieval by text label | Already have           | TODO   |
| [#9](https://github.com/rainwl/MLP/issues/9)   | Retrievel by sketch     | ..                     | TODO   |
| [#10](https://github.com/rainwl/MLP/issues/10) | Preview of model        | Already have           | TODO   |

## Generate features

| Issue                                          | Description                                                 | Remark | Status |
|------------------------------------------------|-------------------------------------------------------------|--------|--------|
| [#11](https://github.com/rainwl/MLP/issues/11) | Automaticlly identified                                     | ..     | TODO   |
| [#12](https://github.com/rainwl/MLP/issues/12) | Automatically generate text labels and projection labels    | ..     | TODO   |
| [#13](https://github.com/rainwl/MLP/issues/13) | Automatically categorize and place in different directories | ..     | TODO   |

## Model function

| Issue                                          | Description                                                                      | Remark | Status |
|------------------------------------------------|----------------------------------------------------------------------------------|--------|--------|
| [#18](https://github.com/rainwl/MLP/issues/18) | Realize the projection of the 3D model in the main, overhead and left directions | ..     | TODO   |
| [#19](https://github.com/rainwl/MLP/issues/19) | Capable of continuous cutting in three directions with three fundamentals        | ..     | TODO   |
| [#20](https://github.com/rainwl/MLP/issues/20) | Assembly disassembly animation, intersecting, cutting, etc                       | ..     | TODO   |

