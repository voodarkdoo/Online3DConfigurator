# ProductVisualization

![Image from Ford Configurator, developed in three.js](images/ford-configurator.jpg)

READ CAREFULLY this document BEFORE you start!

## Prerequisites

- read carefully all slides and notes up to lecture 20 before you start. Try the proposed exercises. 

## Hints

- Try to work out a basic project which satisfies all requirements well before the deadline and as soon as possible: you will then use the remaining time to refine, improve and polish.
- If you are stuck for too much time on a problem, ask for help, preferably in the forum.
- the process is as important as the result. Use this project to learn a workflow, and how to use tools effectively. Experiment, and try to come up with efficient, elegant, and well commented code.
- commit often in your git repository and with meaningful comments.
- do not choose too complex products with many materials. 3-4 materials are enough.


## Goals

The well-known ACME company has asked you to build a product **Web visualizer / configurator** for its new e-commerce site. Before giving you the job, ACME wants to evaluate how faithfully you can visualize and configure products.  ACME sells everything, so you can choose whatever kind of product you want for the demonstration.

Your goal is to build a Web application (a HTML page) that:

- visualizes a product in 3D using three.js, using PBR equations and materials;
- allows the user to inspect the product (e.g. by orbiting the camera around it), and change some material on it by choosing from a few alternatives.

Try to make it look like a simple, but real portion of an e-commerce site, not a three.js example: choose carefully colors, fonts, images, and icons, also taking inspiration from real web sites. Before starting, search the web for existing 3D configurators. Note down what you like and don't like, and try to produce a result as professional as possible.

## Steps (read CAREFULLY)

1. Prepare, and add to the repository, a journal.md file for logging your progress and choices.

2. Choose a product for which: (i) you can easily build a 3D model, or (ii) you can download a 3D model which you have the right to use in non-commercial applications. The model should not be too complex (not more than 100k vertices) and in some format that three.js can read. [Three.js examples](https://threejs.org/examples/) provide a list of loaders for different formats: beware that not all of them work perfectly, and you might have to try with different formats. Preferably, use GLTF, but any other format is ok.

3. Design the lighting for the product. Products in web sites and catalogues are photographed using strategically placed lights that enhance details and shape. For example, [searching google images for product photography lighting](http://www.google.com/images?q=product+photography+lighting) will show you a number of real-world lighting setups that are used for products. In your lighting setup, you can use whatever you want, from punctual lights, to environment map, or light maps, or any combination of them, but you *must include* an environment map.

4. Design the PBR materials for the product. You can use PRB textures found anywhere, or produce them, e.g. with Substance Designer or B2M. If you use textures authored by someone else, just make sure you have the rights for using them in our context (non-commercial application). At least one of the materials must have 2-3 alternatives (e.g. different colors, or materials).

5. Include tone mapping and, if needed, post-processing/color correction.

6. Build the application that renders the chosen 3D model, with the designed lighting setup and materials, and an user interface for selecting the material between the alternatives. You must use shaders written by you, e.g. by extending the shaders we saw in the classroom. Your report needs to describe the kind of BRDF / lights you have implemented.

7. If possible, try to take into account implicit requirements as well. For example, you cannot use textures with file sizes of dozens of megabytes for a Web site; and also, your page should render at least at 30 fps on average smartphones. You will get bonus points for a result that could be deployed to a Web site with few or no modifications.

8. (optional) include any technique that was not explained in the classroom, e.g. some special shader or post-processing technique. This will award you extra points in the evaluation.

9. Write a concise report by overwriting this file.

## Starting code

There is no specific starting code for this project. 

## Documenting and report

For project documentation and reporting, we use the [markdown format](https://daringfireball.net/projects/markdown/syntax), which is also the format of this document. Markdown is a lightweight markup language with plain text formatting syntax which is easy and quick to write, very human-readable, and that can be converted to HTML.

If you need more features than the ones that markdown provides (e.g. writing equations), you can use one of its extensions called [markdeep](https://casual-effects.com/markdeep/).

You are required to document your project in two ways:

- maintain a journal (in a file called journal.md) describing key design decisions, changes, bug symptoms and solutions, including screenshots.
- create a report (by overwriting this file).

The report should be as brief as possible while covering the following points:

- overall description: what your project is about and the files it uses.
- results, including images of the scenes created, taken in a way that clearly illustrates that they satisfy the specification.
- brief explanation of the process that you used to make your scene. Include tools, assets, and planning steps.

## Constraints

If you use textures / 3D models / substances / ..., make sure that you have the rights to include them. For example, search for images that come with a [CC Attribution, ShareAlike or NonCommercial licences](https://creativecommons.org/share-your-work/licensing-types-examples/).

In this project, you are allowed to re-use assets taken elsewhere, but **entirely copying** others' work, even with slight modifications, is forbidden and will have serious consequences beyond the deletion of your project. In any case, mention any source of inspiration in your journal and final report.

## Credits

The image above comes from a [Ford car configurator built in three.js](http://www.ford.com/cars/mustang/customizer/#!/customize).
