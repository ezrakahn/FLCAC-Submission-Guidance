# Appendix: Publishing Data With Collaboration Server

Once your datasets are formatted in the openLCA desktop
application and all metadata fields are completed, the datasets can be
synced to the FLCAC Collaboration Server for publication. The first
time you sync your data to the FLCAC Collaboration Server, you will
first need to obtain a user account and a repository with the LCA Commons.

An overview of the Review phase is as follows:

  - **Obtain Server Account**: If not yet an existing user, the FLCAC
    Platform Administrator will set up the FLCAC Collaboration Server
    account for the submitting agency

  - **Commit to Private Server Repository**: Commit your datasets from
    an openLCA database to a private repository on the Collaboration
    Server

  - **Curate Data** on Server: agency team may use the Collaboration
    Server editorial features to communicate edits and finalize the
    private version of the datasets on the platform

  - > ![](./media/image5.png)

  - **Figure 6. Fetch and commit practices between team members on the
    FLCAC server**

  - 
#### <span class="smallcaps">Login</span>

After you have completed the preliminary sign up tasks, you can
familiarize yourself with the server navigation and features. First, you
may login to the FLCAC Collaboration Server portal.

![](./media/image7.png)

**Figure 6. FLCAC Portal Login**

#### <span class="smallcaps">Default Viewer</span>

Once you login to the portal, the viewing window is different and a list
of repositories will be the central default display.

![](./media/image8.png)

**Figure 7. Default view for FLCAC Collaboration Server Members**

#### <span class="smallcaps">Repositories & Groups List View</span>

You can switch between viewing a list of repositories and that of
repository groups on the left-hand side of the portal.

![](./media/image9.png)

**Figure 8. Toggle Repository Groups view for FLCAC Members**

#### <span class="smallcaps">Add a New Repository</span>

Select a group to view the contained repositories and/or add a new
repository. Creating a new repository allows you to designate in which
Group the repository will be housed via a pull-down menu. Note that you
will only have access to the groups to which you have been assigned
roles.


#### <span class="smallcaps">Syncing Data from openLCA to the Server</span>

Once you have created your repository on FLCAC, you can sync your data
to and use the features of the Collaboration Server.

1)  First, ensure that you have collaboration enabled in your openLCA
    desktop application preferences by checking the “Enable
    collaboration” box in ***“File \> Preferences.”***

![](./media/image11.png)

**Figure 10. Enable collaboration in openLCA desktop**

2)  **Credentials:** Under “User,” you may need to enter your assigned
    Collaboration Server username ID and password credentials that were
    assigned during Onboarding by the FLCAC Platform Administrator.

> **Server URL: https://www.lcacommons.gov/lca-collaboration**
> 
> **User: Your Username**
> 
> **Password: Your Password**

3)  **Connect:** Next, navigate to your database in openLCA, right-click
    on the database and select ***“Repository \> Connect to
    Repository.”***

![](./media/image12.png)

**Figure 11. Connect openLCA database to FLCAC repository**

4)  **Designate:** Then, you designate which repository to which to
    connect. You will name the repository exactly as it is in the URL at
    the Collaboration Server. Adjust the repository path to reflect the
    group and repository name using the syntax:
    “Group\_Name/Repository\_Name”.

![](./media/image13.png)

**Figure 12. Adjusting the openLCA repository connect pathname**

![](./media/image14.png)

**Figure 13. Group and repository name locations**

You will know that your desktop database is connected to the server by
the URL in the database name.

![](./media/image15.png)

**Figure 14. Repository-connected database in openLCA**

5)  **Commit:** Now that your openLCA desktop application is connected
    to the server repository, you can commit the data to the server
    repository by right-clicking on the database and selecting
    ***“Repository \> Commit.”*** You should see the commit window
    appear.

![](./media/image16.png)

**Figure 15. Commit changes to a repository**

**Commit, cont.:** You must select the entities you wish to commit and
enter a commit message. Best practices for commit messages include short
phrases indicating the datasets being committed. The commit message will
display next to each dataset committed in the Collaboration Server (see
next page) and if the message is extensive, it will affect the ease of
navigation through the data as it displays on the server.

If you are committed a large number of datasets for the first time, the
commit action can take some time (minutes up to an hour for very large
datasets). However, once the repository is established, updates may be
committed in seconds. For reference, the entire USLCI Database takes
about four minutes to commit to a new repository. You should see
messages indicating that the application is:

  - Searching for referenced changes

  - Checking against libraries

  - Committing changes

  - Estimated time: \# minutes

  - Indexing datasets

![](./media/image17.png)

![](./media/image18.png)

**Figure 16. Progress indicators for database change commits**

6)  **View Commits:** Once the repository is committed, you should be
    able to navigate to your repository on the Collaboration Server and
    verify the presence of your datasets, when the change was made, and
    the commit message.

![](./media/image19.png)

**Figure 17. Viewing commits on the FLCAC portal**
