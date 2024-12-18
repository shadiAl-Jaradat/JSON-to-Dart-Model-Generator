# JSON-to-Dart Model Generator Feature in Nowa : 
Developed and enhanced a Flutter-powered desktop and web app for a no-code platform, enabling users to generate mobile apps with Flutter as the underlying source code. My work spanned coding, product strategy, feature identification, user experience optimization, and ensuring high performance and stability across the platform. and Here’s a main fetures that I proud of.


## Table of content 

1. [Overview](#overview-)
2. [Video](#video-)
3. [High Level Architecture](#high-level-architecture)
4. [How it works](#how-it-works)
5. [Feature Highlights](#feature-highlights)
6. [Solution Design Process](#solution-design-process)


## Overview :
I designed and implemented a JSON-to-Dart model generator for a no-code platform built using Flutter. This feature transforms JSON input into structured Dart classes, streamlining the development of Flutter apps by generating reusable models automatically. My work involved integrating multiple functionalities such as interactive JSON editing, custom tree views, and conflict-free model generation, focusing on enhancing the user experience and optimizing code reliability.

I’m incredibly proud of this feature because it highlights my technical skills and ability to deliver end-to-end solutions. However, the code is confidential, so I cannot share it.

## Video : 

https://github.com/user-attachments/assets/65dd501d-5108-4e2a-bd95-36ab7c4f6775


## High Level Architecture

<img width="942" alt="image" src="https://github.com/user-attachments/assets/2f303caa-780a-4404-8a2d-a355c2f4d52d">


## How it works
1- JSON Input:
  - Users enter JSON in the JsonEditor.
  - The editor validates the JSON and prettifies the format.

2- Data Selection:
  - The JSON structure is visualized as a tree.
  - Users select the relevant data nodes for model generation.

3- Model Generation:
  - The GenerateModelProvider processes the selected JSON and generates Dart model classes using DataGenerator.
  - Users can review, rename, and customize the generated models.

4- Save Models:
  - Models are saved to the specified directory.
  - The models will opened in the editor.


## Feature Highlights:

#### 1- Interactive JSON Editor:

Functionality: Provides an embedded JSON editor that supports prettifying and compressing JSON data.
Implementation: Utilized the re_editor package to build an intuitive editor interface where users can directly input or modify JSON content.
Tech: A structured Tree<JsonNode> is used to parse and manage the JSON data. Each node in the tree maintains a selectable state, controlling data visibility across various sections.

#### 2- Custom Tree Views for Data Selection:

Functionality: Enables users to select specific JSON keys or objects, which populate in another tree structure for generating corresponding Dart classes.
Implementation: Developed with the tree_view package to render interactive and hierarchical views. Each tree node tracks the exact path of its JSON key-value, ensuring precise traversal and accurate model generation.
Conflict Management: Implemented logic to prevent naming conflicts by ensuring that each generated Dart class follows Flutter naming conventions.


#### 3- Dart Model Generation:

Functionality: Converts selected JSON data into Dart models with a modular and reusable design.
Design: The generator avoids duplicate models by checking existing class names and paths, ensuring optimized code structure.
Usability: Users are guided through the generation process with dialog boxes and segmented views to manage the data-to-model workflow seamlessly.
State Management and UI Optimization:

Integration: Leveraged the provider package for state management, ensuring smooth synchronization between the JSON editor, data selection views, and model generation.
Performance: Designed the feature to minimize re-renders and maintain high UI responsiveness during complex data operations.



## Solution Design Process

<img width="1217" alt="Screenshot 2024-10-18 at 1 50 03 PM" src="https://github.com/user-attachments/assets/bdc60311-b08e-44ae-9fce-f13f8c746904">


