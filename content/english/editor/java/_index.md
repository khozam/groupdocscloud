---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Editor"
product_tag: "editor"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Editor Cloud SDK – Edit Word Excel PowerPoint HTML"
head_description: "Work with Java document editor cloud SDK & REST APIs to edit Word, Excel spreadsheets, PPTX, HTML, XML file formats.‎"

############################# Header ############################
title: "Documents Editor SDK for Java Applications"
description: "Document editor REST API to build advanced documents editing and manipulating tools using Java Cloud SDK on web, mobile, desktop or cloud platforms.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Editor Cloud SDK for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_editor-for-java.webp"
        product: "GroupDocs.Editor"
        platform: "JAVA"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "#support-resources"
              text: "Resources"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-java"
        link_learn: "https://docs.groupdocs.cloud/editor/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Editor Cloud SDK for Java easily integrates with GroupDocs.Editor Cloud REST API, allowing to add documents editing features in Java applications without MS Office or other additional applications installed. Using the Java editor SDK – speed up the document manipulation task across a wide range of supported document formats including Microsoft Word, Excel spreadsheets, Presentations, TXT, HTML and XML. Simply fetch the document into any WYSIWYG HTML editor, edit it as needed and save it back to original document formats with true accuracy and efficiency.

      Perform all most demanded document editing operations across the supported file formats. GroupDocs.Editor Cloud SDK for Java is built as a layer on top of GroupDocs.Editor Cloud REST API that saves valuable development time by managing low-level requests and handling responses. The developers can focus on writing up the specific code only as needed in the project.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Editor Cloud SDK for Java requires Java Runtime Environment and can run on any platform where these requirements can be met.

        left:
          enable: true
          icon: "fas fa-align-left"
          title: "Editing Option"
          content: |
            * Edit in flow or parged mode
            * Multi-language document
            * Manage font extraction
            * Support tabbed spreadsheets
            * Memory usage optimization
        
        right:
          enable: true
          icon: "fas fa-sitemap"
          title: "Information Extraction"
          content: |
            * Document Type
            * Document Size
            * Page Count
            
        
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Editor Cloud supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, FlatOPC, ODT, OTT, RTF, WordML
                * **Microsoft Excel**: XLS, XLSX, XLT, XLSM, XLSB, XLTX, XLTM, XLAM, SXC, SpreadsheetML, ODS, FODS, DIF, DSV, CSV, TSV
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX, PPSM, PPTM, POT, POTX, POTM, ODP, OTP

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **Plain Text**: TXT
                * **Markup**: HTML, XML

      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Editor REST API while using your favorite language & platform.
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Advanced Document Editor REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Integrates easily within any WYSIWYG editor"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Edit Word documents as a whole or define pages range"

      # feature loop
      - icon: "fas fa-file-image"
        content: "Multi-tabbed spreadsheet editing is supported"
      
      # feature loop
      - icon: "fas fa-file-alt"
        content: "Optimized memory usage for large CSV or TSV files"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Extract document information (type, size, page count etc)"

      # feature loop
      - icon: "fas fa-folder"
        content: "Cloud REST API to be used with any language or platform"



      

    more_feature:
      # more_feature_loop
      - title: "Working with WordProcessing Documents - Java"
        content: |
          
          ```java
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
          Configuration configuration = new Configuration(MyAppSid, MyAppKey);

          // Create necessary API instances
          EditApi editApi = new EditApi(configuration);
          FileApi fileApi = new FileApi(configuration);
          
          // The document already uploaded into the storage.
          // Load it into editable state
          FileInfo fileInfo = new FileInfo();
          fileInfo.setFilePath("WordProcessing/password-protected.docx");
          fileInfo.setPassword("password");
          WordProcessingLoadOptions loadOptions = new WordProcessingLoadOptions();
          loadOptions.setFileInfo(fileInfo);
          loadOptions.setOutputPath("output");
          LoadResult loadResult = editApi.load(new LoadRequest(loadOptions));
          
          // Download html document
          File file = fileApi.downloadFile(new DownloadFileRequest(loadResult.getHtmlPath(), null, null));
                      
          // Edit something...
          List lines = Files.readAllLines(file.toPath());
          List newLines = new ArrayList();
          for (String line : lines) {
              newLines.add(line.replaceAll("Sample test text", "Hello world"));
          }
          Files.write(file.toPath(), newLines);
          
          // Upload html back to storage
          fileApi.uploadFile(new UploadFileRequest(loadResult.getHtmlPath(), file, Common.MYStorage));
          
          // Save html back to docx
          WordProcessingSaveOptions saveOptions = new WordProcessingSaveOptions();
          saveOptions.setFileInfo(fileInfo);
          saveOptions.setOutputPath("output/edited.docx");    
          saveOptions.setHtmlPath(loadResult.getHtmlPath());      
          saveOptions.setResourcesPath(loadResult.getResourcesPath());
          DocumentResult saveResult = editApi.save(new SaveRequest(saveOptions));
          
          System.out.println("Document edited: " + saveResult.getPath());
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Editor offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Editor for cURL"
          image: "/sdk/272x272/groupdocs_editor-for-curl.webp"
          product: "GroupDocs.Editor"
          platform: "cURL for Cloud"
          link: "/editor/curl/"
          # solution loop
        - img_alt: "GroupDocs.Editor for .NET"
          image: "/sdk/272x272/groupdocs_editor-for-net.webp"
          product: "GroupDocs.Editor"
          platform: ".NET"
          link: "/editor/net/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Java"
          image: "/sdk/272x272/groupdocs_editor-for-java.webp"
          product: "GroupDocs.Editor"
          platform: "Java"
          link: "/editor/java/"
          # solution loop
        - img_alt: "GroupDocs.Editor for PHP"
          image: "/sdk/272x272/groupdocs_editor-for-php.webp"
          product: "GroupDocs.Editor"
          platform: "Php"
          link: "/editor/php/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Python"
          image: "/sdk/272x272/groupdocs_editor-for-python.webp"
          product: "GroupDocs.Editor"
          platform: "Python"
          link: "/editor/python/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Ruby"
          image: "/sdk/272x272/groupdocs_editor-for-ruby.webp"
          product: "GroupDocs.Editor"
          platform: "Ruby"
          link: "/editor/ruby/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Node.js"
          image: "/sdk/272x272/groupdocs_editor-for-node.webp"
          product: "GroupDocs.Editor"
          platform: "Node.js"
          link: "/editor/nodejs/"
          # solution loop
        - img_alt: "GroupDocs.Editor for Android"
          image: "/sdk/272x272/groupdocs_editor-for-android.webp"
          product: "GroupDocs.Editor"
          platform: "Android"
          link: "/editor/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---