Compgen Course 2025
===================

Here I collect relevant course material for the Computational Genomics Course (10-16 March 2025), Module 3.
In this module, we learn about how to use deep learning models to integrate multi-omics data in the context of precision oncology applications.
See here the tool (Flexynesis) that we use throughout this course: https://github.com/BIMSBbioinfo/flexynesis. 

Course Material
======================

Here is the course material we have developed during the workshop. Feel free to share and re-use. 

1. Day-1: 

   - `Slides <https://docs.google.com/presentation/d/1Z3m8JOQY0JidM7gIJNFWaOfCaTH-rU47y4zCu5Bk6mE/edit?usp=sharing>`_
   - `Live session <https://youtu.be/7QxRqhFDJiY?feature=shared>`_
   - `Homework <https://github.com/BIMSBbioinfo/compgen_course_2025_module3/tree/main/homeworks/hw1>`_
   - `Homework solutions <https://github.com/BIMSBbioinfo/compgen_course_2025_module3/blob/main/solutions/day1_hw_brca_subtypes_solutions.ipynb>`_

2. Day 2: 

   - `Slides <https://docs.google.com/presentation/d/1a31RoNIiZYdZFL9cc4OZ3TpgBGrk1IH1brW9VeHo3dQ/edit?usp=sharing>`_
   - `Live session <https://youtu.be/CjTjcu_k2EI?feature=shared>`_
   - `Homework <https://github.com/BIMSBbioinfo/compgen_course_2025_module3/tree/main/homeworks/hw2>`_
   - `Homework solutions <https://github.com/BIMSBbioinfo/compgen_course_2025_module3/blob/main/solutions/day2_hw_lgg_gbm_solutions.ipynb>`_ 

3. Day 3: 

   - `Slides <https://docs.google.com/presentation/d/1OvXK4H5W7qbD4jeru8pwnkQdiGz0RfjrW4Omd8kd0dg/edit?usp=sharing>`_
   - `Live session <https://youtu.be/WM4VkjFHOwI?feature=shared>`_
   - `Homework <https://github.com/BIMSBbioinfo/compgen_course_2025_module3/tree/main/homeworks/hw3>`_
   - `Homework solutions <https://github.com/BIMSBbioinfo/compgen_course_2025_module3/tree/main/solutions/hw3>`_ 

4. Day 4: 

   - `Live session <https://youtu.be/jYzKw4rF-ck?feature=shared>`_
   - We didn't use any slides and we didn't have any more homeworks. 
   

Compute Environment
===================

Cloud - Rolv.io
---------------

You will be provided usernames and passwords to access the `rolv.io` platform, which comes with prebuilt packages that you will need throughout the course. With this option, you won't need to install any software yourself.

Please check your email that you signed up for the course, use your credentials to sign in: `Rolv.io Platform <https://platform.dev.cloud.rolv.io/>`_.
Then, click on **Compute -> Launch -> Launch JupyterLab**. Wait for the session to be ready (takes a few minutes).
There you will have a JupyterLab environment with all packages installed.
In this session, you can also use the **terminal**.

+++++++++++++++++++++

**Important Note**: Each session you create on Rolv is **limited** to a **total of 3 hours**. 
Please make sure to **backup your work** before terminating your session. 
We recommend creating a github repo and have a backup of your work there. 

+++++++++++++++++++++

Docker Desktop
---------------

We have also built a Docker image that contains the tools you will need.
To be able to use this, you need Docker Desktop, which you can install from here: `Docker Desktop <https://www.docker.com/products/docker-desktop/>`_.

After you install Docker, open a terminal and execute the following code to open a JupyterLab session with all the tools you need:

.. code-block:: bash

   docker pull borauyar/flexynesis_image:latest
   docker run -it -p 8888:8888 borauyar/flexynesis_image
   jupyter lab --ip=0.0.0.0 --no-browser --allow-root

This will create a link that looks like this:

   http://127.0.0.1:8888/lab?token=<.......>

Copy-paste that link into your browser to open a JupyterLab session.

Mamba/pip
---------------

If you want to have more control over your system and you know what you are doing, you can also install **flexynesis** on your system using `pip`.

.. code-block:: bash

   mamba create -n flexenv python==3.11
   mamba activate flexenv
   pip install flexynesis jupyterlab snakemake
   jupyter lab --ip=0.0.0.0 --no-browser --allow-root

This will create a link that looks like this:

   http://127.0.0.1:8888/lab?token=<.......>

Copy-paste that link into your browser to open a JupyterLab session.

Further Learning
===================

Here are some resource I found useful: 

- Fastai: https://course19.fast.ai/part2
- Pytorch: https://pytorch.org/tutorials/index.html
- Lightning: https://www.datacamp.com/tutorial/pytorch-lightning-tutorial
- Pytorch-Geometric for GNNs: https://pytorch-geometric.readthedocs.io/en/latest/ 
- Graph Neural Networks: https://www.youtube.com/watch?v=fOctJB4kVlM&list=PLV8yxwGOxvvoNkzPfCx2i8an--Tkt7O8Z&ab_channel=DeepFindr
- Elements of statistical learning (Rob Tibshirani, Trevor Hastie): https://www.youtube.com/watch?v=LvySJGj-88U&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&ab_channel=StanfordOnline
- Computational Genomics in R (Akalin, Franke, Ronen, Uyar): https://compgenomr.github.io/book/










