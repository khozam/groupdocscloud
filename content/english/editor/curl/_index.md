---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Editor"
product_tag: "editor"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "GroupDocs.Editor Cloud for cURL"
head_description: "Work with cURL commands to access the REST APIs for editing popular document formats such as Microsoft Office TXT, HTML and XML.‎"

############################# Header ############################
title: "Editing Document Formats using cURL"
description: "Work with cURL commands to access the REST APIs for editing popular document formats such as Microsoft Office TXT, HTML and XML.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Editor Cloud for cURL"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_editor-for-curl.png"
        product: "GroupDocs.Editor"
        platform: "cURL"

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
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://groupdocscloud.github.io/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Editor Cloud for cURL makes it possible for you to quickly access GroupDocs REST APIs using cURL commands and edit contents of popular document file formats keeping the layout and appearance of the documents undisturbed. Simply upload the source document into any HTML editor of your choice, manipulate the document and save the resultant document back into the original format.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Editor Cloud for cURL.

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
          GroupDocs.Editor Cloud allows editing a a variety of document formats.

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
          GroupDocs.Editor Cloud for cURL - some of the supported languages and platforms.
        
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
      - title: "Load Excel Spreadsheet Document using cURL"
        content: |
          
          ```shell
          curl -v "https://api.groupdocs.cloud/v1.0/editor/load" \
          -X POST \
          -H "Content-Type: application/json" \
          -H "Accept: application/json" \
          -H "Authorization: Bearer 
          "
          -d "{
              'FileInfo': { 'FilePath': 'Spreadsheet/four-sheets.xlsx' },
            'OutputPath': 'Output',
            'WorksheetIndex': 0
          }"
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
          platform: "cURL"
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