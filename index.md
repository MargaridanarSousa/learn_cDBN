## learn_cDBN

learn_cDBN is a Java implementation of a learning algorithm for **consistent k-graph dynamic Bayesian networks**(cDBN). The program receives a data set with multivariate longitudinal categorical observations and outputs the optimal structure. The algorithm has polynomial time complexity in the number of attributes and observations. 

If you use learn_cDBN is your research please cite:

José L Monteiro, Susana Vinga, and Alexandra M Carvalho. [Polynomial-time algorithm for learning
optimal tree-augmented dynamic Bayesian networks.](http://auai.org/uai2015/proceedings/papers/329.pdf) In UAI, pages 622–631, 2015.

## Usage

In [tDBN](http://josemonteiro.github.io/tDBN/) the input file format is described.

By executing the following .jar file:
```
$ java -jar learn_cDBN.jar

```

The command line options are:
```


 -c,--compact                 Outputs network in compact format, omitting
                              intra-slice edges. Only works if specified
                              together with -d and with --markovLag 1.
 -d,--dotFormat               Outputs network in dot format, allowing
                              direct redirection into Graphviz to
                              visualize the graph.
 -i,--inputFile <file>        Input CSV file to be used for network
                              learning.
 -m,--markovLag <int>         Maximum Markov lag to be considered, which
                              is the longest distance between connected
                              time-slices. Default is 1, allowing edges
                              from one preceding slice.
 -ns,--nonStationary          Learns a non-stationary network (one
                              transition network per time transition). By
                              default, a stationary DBN is learnt.
 -o,--outputFile <file>       Writes output to <file>. If not supplied,
                              output is written to terminal.
 -p,--numParents <int>        Maximum number of parents from preceding
                              time-slice(s).
 -pm,--parameters             Learns and outputs the network parameters.
 -r,--root <int>              Root node of the intra-slice tree. By
                              default, root is arbitrary.
 -s,--scoringFunction <arg>   Scoring function to be used, either MDL or
                              LL. MDL is used by default.
 -sp,--spanning               Forces intra-slice connectivity to be a tree
                              instead of a forest, eventually producing a
                              structure with a lower score.
                              
 -ckg,---ckg                  boolean, if true learns cDBN structure,
                              else, learns tDBN structure.
                              
 -ind,---intra_ind            In-degree of the intra-slice transition 
                              network.
                                                       
```




## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/MargaridanarSousa/learn_cDBN/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/MargaridanarSousa/learn_cDBN/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
