# PMO - a maven archetype for creating a directory layout used for project administration.

I admit this is quite overblown as a simple shell script would have done
the trick, but I liked the idea just for training purpose (while creating
my very first maven archetype)

# Usage

Clone this directory and do a 

    mvn install -DskipTests=true

after that you have the archetype available in your local maven repository.

Now when you encounter a new project as project manager, go to your projects parent dir
and in this directory you do a 

    mvn archetype:generate \
    -DgroupId=your.company \
    -DartifactId=yourProjectName \
    -Dversion=1.0-SNAPSHOT \
    -DarchetypeGroupId=de.bluewhale.archetypes \
    -DarchetypeArtifactId=PMO

Answer the prompted question with 'Y'
Afterwards you have the dummy project pmo layout in the new created directory 'youProjectName'

# Customize

Of course this is a layout I use, you may want to give it your own flavor. 
The best way to do so is to fork this project to customize it to your needs.
Merge requests won't be accepted.