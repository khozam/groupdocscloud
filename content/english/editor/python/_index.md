---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Editor"
product_tag: "editor"
platform: "Python"
platform_tag: "python"

############################# Head ############################
head_title: "Python Document Editor Cloud SDK to edit Word Excel HTML XML"
head_description: "Document editor Python Cloud SDK and REST API to edit business document formats including Microsoft Word, Excel, HTML, XML and PowerPoint presentations.‎"

############################# Header ############################
title: "Python Document Editor REST API & SDK"
description: "Document editor REST API to edit popular document formats using any WYSIWYG HTML editor without asking to install external applications."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Editor Cloud SDK for Python"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_editor-for-python.webp"
        product: "GroupDocs.Editor"
        platform: "Python"

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
        link_download: "https://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-python"
        link_learn: "https://docs.groupdocs.cloud/editor/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Editor Cloud SDK for Python makes it easier for developers to incorporate document editing features within Python based applications by integrating it with GroupDocs.Editor Cloud REST API. Perform advanced document editing operations by simply fetching the supported document types (Microsoft Word, Excel spreadsheets, PowerPoint, TXT, HTML, XML) in any front-end HTML editor using GroupDocs.Editor Cloud API and save it back to original document format after editing the document.

      GroupDocs.Editor Cloud SDK for Python is built as a layer on top of GroupDocs.Editor Cloud REST API that saves valuable development time by managing low-level requests and handling responses. The developers can focus on writing up the specific code only as needed in the project.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Editor Cloud SDK for Python requires Python 2.7 or 3.4 or later.

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
      - title: "Working with WordProcessing Documents - Python"
        content: |
          
          ```py          
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
            editApi = groupdocs_editor_cloud.EditApi.from_keys(app_sid, app_key)
            fileApi = groupdocs_editor_cloud.FileApi.from_keys(app_sid, app_key)
            
            # The document already uploaded into the storage.
            # Load it into editable state
            fileInfo = groupdocs_editor_cloud.FileInfo("WordProcessing/password-protected.docx", None, None, "password")
            loadOptions = groupdocs_editor_cloud.WordProcessingLoadOptions()
            loadOptions.file_info = fileInfo
            loadOptions.output_path = "output"
            loadResult = editApi.load(groupdocs_editor_cloud.LoadRequest(loadOptions))        
            
            # Download html document
            htmlFile = fileApi.download_file(groupdocs_editor_cloud.DownloadFileRequest(loadResult.html_path))
            html = ""       
            with open(htmlFile, 'r') as file:
                html = file.read()
            
            # Edit something...    
            html = html.replace("Sample test text", "Hello world")
            
            # Upload html back to storage
            with open(htmlFile, 'w') as file:
                file.write(html)
            
            fileApi.upload_file(groupdocs_editor_cloud.UploadFileRequest(loadResult.html_path, htmlFile))
            
            # Save html back to docx
            saveOptions = groupdocs_editor_cloud.WordProcessingSaveOptions()
            saveOptions.file_info = fileInfo
            saveOptions.output_path = "output/edited.docx"
            saveOptions.html_path = loadResult.html_path
            saveOptions.resources_path = loadResult.resources_path
            saveResult = editApi.save(groupdocs_editor_cloud.SaveRequest(saveOptions))

            # Done
            print("Document edited: " + saveResult.path)
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