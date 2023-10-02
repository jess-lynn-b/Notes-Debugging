# Understanding Angular Error Messages

    Always keep the developer console open. This will help you spot errors and be able to catch them as the happen or at least quickly.

    The first part tells you where the error is located and then the next tells you what line you can find the error on. Finally it tells you what the error is and what it could be missing and how to fix. 

    Do not panic and if at a loss always google...it can help as well

# Debugging code in the browser using sourcemaps

    If reading error messages is not enough to help... it may not be an error messgae but simply a logical erro in the app. For this we can use debugging. 

    In developer tools in chrome you can go to sources imported on this page. Then you can see all the script bundles and there are a couple you see, the impt one for us is the main bundle. In the main bundle we can see the templaate with container and row and then try to locate the line responsible for splicing. You can debug here but it might jump to the app. comp. ts file. Bc TS is not what runs the browser but the JS bundles are used. 

    Sourcemaps are a little addition to the CLI and adds bundles which allow the browser to translate JS to TS. 

    If you want to access the TS files directly you can under the webpack cloud off to the side of the developer tools and then choose the subfolders. 