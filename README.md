# Xtext Editor for EAST-ADL with Artifacts Relevant for the MODELSWARD'23 Position Paper "Exploiting Meta-Model Structures in the Generation of Xtext Editors"
This repository contains an Xtext-based editor for a textual concrete syntax of the EAST-ADL meta-model, called EATXT. The editor is used to explore what a textual syntax for EAST-ADL can look like and contains artifacts and examples as demonstrations means for the MODELSWARD'23 Position Paper "Exploiting Meta-Model Structures in the Generation of Xtext Editors".

## Setting Up the Development Workspace
1. Get an Eclipse Modeling Tools
1. In this Eclipse, install the additional component "Xtext Complete SDK"
1. Clone the repository at hand
1. Import <code>releng/org.bumble.eatxt.target</code> and load its target definition <code>org.bumble.eatxt.target.target</code>
1. Import all plugins in the folder <code>plugins</code>
   - If build paths of some of these plugins are not correct as folders like <code>src-gen</code> or <code>xtend-gen</code> are missing, just create corresponding empty folders in these plugins via right-click -> New -> Folder. 
   Their contents are generated later.
1. In the project <code>org.bumble.eatxt</code>, open the equally named source folder, right-click on <code>Eatxt.xtext</code>, and select "Run as" -> "Generate Xtext Artifacts"
1. After the Xtext infrastructure is generated, start the Eclipse runtime instance

## Setting Up the Runtime Workspace
1. Import the project <code>examples/org.bumble.eatxt.examples</code>
1. Experiment with the file <code>MODELSWARD23.eatxt</code>.

## Artifacts Relevant for the MODELSWARD'23 Position Paper "Exploiting Meta-Model Structures in the Generation of Xtext Editors"
As explained in the paper, there are the following relevant artifacts in the project <code>org.bumble.eatxt</code>:
1. <code>src/org.bumble.eatxt.templates/EatextTemplateFragment.xtend</code>: Described in Section 4.1
1. <code>src/org.bumble.eatxt.contentassist/EatextContentAssistFragment.xtend</code>: Described in Section 4.2
1. <code>src/org.bumble.eatxt.formatting2/EatxtFormatter2Fragment.xtend</code>: Described in Section 4.3
1. <code>src/org.bumble.eatxt/Activator.java</code>: Described in Section 4.4
