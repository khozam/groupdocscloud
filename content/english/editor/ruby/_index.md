---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Editor"
product_tag: "editor"
platform: "Ruby"
platform_tag: "ruby"

############################# Head ############################
head_title: "Ruby Document Editor Cloud SDK – Edit Word Excel HTML XML PPTX"
head_description: "Document editor Ruby Cloud SDK and REST APIs to build apps with document editing features. Edit Microsoft Word, Excel, HTML, XML and PPTX file formats.‎"

############################# Header ############################
title: "Documents Editor SDK for Ruby Applications"
description: "Cloud REST API to incorporate document editing features within Ruby applications. No external application needed to edit documents of all popular formats."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Editor Cloud SDK for Ruby"
        image: "/sdk/272x272/groupdocs_editor-for-ruby.webp"
        product: "GroupDocs.Editor"
        platform: "Ruby"

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
        link_download: "https://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-ruby"
        link_learn: "https://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-ruby"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Editor Cloud SDK for Ruby is easy to integrate with GroupDocs.Cloud REST API, thus allowing to quickly edit a wide range of document formats within Ruby applications without needing to install MS Office or other applications. Using the document editor library – easily perform all most demanded document editing operations while manipulating presentations, Excel spreadsheets, HTML, XML and Word processing documents. Just upload the document file to be edited via GroupDocs.Editor Cloud API into any front-end WYSIWYG editor, manipulate it and easily convert back to its original document type.

      GroupDocs.Editor Cloud SDK for Ruby is built as a layer on top of GroupDocs.Editor Cloud REST API that saves valuable development time by managing low-level requests and handling responses. The developers can focus on writing up the specific code only as needed in the project.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Editor Cloud SDK for Ruby has the following requirements:

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
      - title: "Working with Presentations - Ruby"
        content: |
          
          ```rb          
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
            fileApi = GroupDocsEditorCloud::FileApi.from_keys($app_sid, $app_key)
            editApi = GroupDocsEditorCloud::EditApi.from_keys($app_sid, $app_key)
            
            # The document already uploaded into the storage.
            # Load it into editable state
            fileInfo = GroupDocsEditorCloud::FileInfo.new
            fileInfo.file_path = 'Presentation/with-notes.pptx'       
            
            loadOptions = GroupDocsEditorCloud::PresentationLoadOptions.new
            loadOptions.file_info = fileInfo
            loadOptions.output_path = "output"
            loadOptions.slide_number = 0
            
            loadRequest = GroupDocsEditorCloud::LoadRequest.new(loadOptions)        
            loadResult = editApi.load(loadRequest)
            
            # Download html document
            htmlFile = fileApi.download_file(GroupDocsEditorCloud::DownloadFileRequest.new loadResult.html_path)
            htmlFile.open
            html = htmlFile.read
            htmlFile.close
            
            # Edit something...
            html = html.gsub("Slide sub-heading", "Hello world!")
            
            # Upload html back to storage
            htmlFile = File.open(htmlFile.path, "w")        
            htmlFile.write(html)
            htmlFile.close
            uploadRequest = GroupDocsEditorCloud::UploadFileRequest.new loadResult.html_path, File.open(htmlFile.path, "r")
            fileApi.upload_file(uploadRequest)
            
            # Save html back to pptx
            saveOptions = GroupDocsEditorCloud::PresentationSaveOptions.new
            saveOptions.file_info = fileInfo
            saveOptions.output_path = "output/edited.pptx"
            saveOptions.html_path = loadResult.html_path
            saveOptions.resources_path = loadResult.resources_path
            
            saveRequest = GroupDocsEditorCloud::SaveRequest.new(saveOptions)
            saveResult = editApi.save(saveRequest)        
            
            puts("Document edited: " + saveResult.path)
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