## Project Layout

Choosing a project layout has a surprising number of consequences for a team. The Java approach and conventional wisdom separatea projects along language and environment seams. There are separate folders for `main/` and `test/`, and separate folders for language, `src/scala/com/...` and `src/java/...`. Rails and Rails-likes split the project along OO seams, creating different directories for `app/` and `test/`. Inside `app/` and `test/` are folders for `controllers/` and `templates/`. These approaches place the framework concepts front and center, forcing developers to think about the tools first and the business model second. To go from a controller to a template requires navigating up and then back down the directory structure.

A better conceptual approach is to break the application along business model seams. There are good reasons for doing so. It places the conceptual model of the business itself at the forefront of development. This allows easier mix & match of the various transpiled languages. Putting the business model and logic first builds in a ubiquitous language for the project, a useful concept from the field of Domain Driven Development. Team members see their business components first, and talk about the specific controller, schema, or template later. While mixing languages makes the build tools take more configuration, it usually falls to the difference in moving `coffee/**` to `**/*.coffee`. Teams can choose languages that are most comfortable to their style concerns.

### Components
1. **Deploy**
1. **Server**
1. **Client**
1. **Features**

### Languages

1. **script**: *JavaScript* vs *Coffee* vs *Dart*
1. **markup**: *HTML* vs *Jade*
1. **styling**: *css* vs *Stylus* vs *SASS* vs *Less*

### Build Toolchain

1. **Grunt** *Task Configuration*
1. **Gulp** *Build Pipelines*
1. **Closure Compiler** *Static type safety*

### Static Typing
