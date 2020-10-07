# pandana-urbanaccess-issue

This repo contains notebooks invesetigating a reported issue where adding a subway network in UrbanAccess/Pandana had the unexpected effect of _reducing_ accessibility (jobs within 15 minutes) for certain locations.

The cause turned out to be a workflow bug: when job counts are linked up to network nodes, they need to be linked to nodes that exist in both networks to achieve consistent results. For full details, see [Accessibility-solution.ipynb](https://github.com/ual/pandana-urbanaccess-issue/blob/main/Accessibility-solution.ipynb).

The second notebook ([Transit-route-quality.ipynb](https://github.com/ual/pandana-urbanaccess-issue/blob/main/Transit-route-quality.ipynb)) confirms that the routing itself is working as expected.

These notebooks may also be useful as code examples for related tasks.

### Environment

Python 3.8  
NumPy 1.19  
Pandas 1.1  
Matplotlib 3.3  
Pandana 0.5  
UrbanAccess 0.2  
Jupyter  
nb_conda_kernels
