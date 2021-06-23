---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Merger"
product_tag: "merger"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Merge & Split Documents with cURL Commands"
head_description: "Simple cURL commands to separate or combine documents like PDF, Word documents, Excel spreadsheets, presentations, HTML and many supported file formats."

############################# Header ############################
title: "Merge and Split Documents using cURL"
description: "Document merge or split using simple cURL commands for REST APIs. Reliably rotate, tilt, change orientation, reorder document pages of any file format."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Merger Cloud for cURL"
        image: "/sdk/272x272/groupdocs_merger-for-curl.webp"
        product: "GroupDocs.Merger"
        platform: "Cloud for cURL"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/merger/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/merger/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Merger Cloud API provides a solution to split and merge documents of all common business formats. Using cURL, you can perform many others operation by just sending requests to the REST API and receive responses to manipulate documents in the cloud. Supported file types include; PDF, Microsoft Word documents, Excel spreadsheets, PowerPoint presentations, OpenDocument formats, plain text and others.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document merger Cloud API.
      
        left:
          enable: true
          icon: "fas fa-file"
          title: "Single Document Operations"
          content: |
            * Join multiple pages
            * Split document
            * Document pages preview
            * Change page order
            * Change page orientation
            * Extract pages
            * Remove pages
            * Rotate pages
            * Swap any two pages
        right:
          enable: true
          icon: "fas fa-files-o"
          title: "Multiple Files Operations"
          content: |
            * Combine multiple documents into one
            * Add document password
            * Update document password
            * Remove document password
            * Check document for password protection
      
      ## TAB TWO ##
      tab_two:
        description: |
          Document merger Cloud API supported formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**:  XLS, XLSX, XLSM, XLSB, XLT, XLTM, XLTX
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Visio**: VDX, VSDX, VSDM, VSX, VSSX, VSSM, VTX, VSTX, VSTM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Other Formats"
              content: |
                * **OpenDocument Formats**: ODT, OTT, ODP, OTP, ODS
                * **Fixed Layout**: PDF, XPS
                * **Text**: TXT, RTF, CSV, TSV
                * **Web**: HTML, MHT
                * **LaTex**: TEX
                * **eBook**: EPUB


      ## TAB THREE ##
      tab_three:
        description: |
          Supported Operating Systems and Frameworks
      
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
    title: "Document Merger REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-files-o"
        content: "Combine multiple pages, slides or spreadsheets into a single document"

      # feature loop
      - icon: "fas fa-random"
        content: "Swap position of any two pages, slides or sheets within a document"

      # feature loop
      - icon: "fas fa-repeat"
        content: "Rotate pages by setting rotation angles like 90, 180 or 270 degrees"
      
      # feature loop
      - icon: "fas fa-scissors"
        content: "Split any document into smaller files"

      # feature loop
      - icon: "fas fa-times"
        content: "Remove any single or collection of specific pages"

      # feature loop
      - icon: "fas fa-refresh"
        content: "Change page orientation"

      # feature loop
      - icon: "fas fa-sort-amount-asc"
        content: "Rearrange pages, slides or diagrams"

      # feature loop
      - icon: "fas fa-key"
        content: "Set, reset & remove password"

      # feature loop
      - icon: "fas fa-list"
        content: "Fetch list of supported file formats"
    
    more_feature:
      # more_feature_loop
      - title: "Merge multiple documents"
        content: "Using GroupDocs.Merger Cloud API, you can combine two or more documents into one document, or split any document into multiple smaller documents. Following simple cURL command shows how to merge two PDF files."

      # more_feature_loop
      - title: "Merge PDF documents - cURL"
        content: |
          
          
          ```shell
          curl -X POST "https://api.groupdocs.cloud/v1.0/merger/join" \
          -H "accept: application/json" \
          -H "authorization: Bearer TOKEN-HERE" \
          -H "Content-Type: application/json" \
              -d "{ \"JoinItems\": [ { \"FileInfo\": { \"FilePath\": \"/foldername/doc1.pdf\", \"StorageName\": \"my Storage\" } }, { \"FileInfo\": { \"FilePath\": \"/foldername/doc2.pdf\", \"StorageName\": \"my Storage\" } } ], \"OutputPath\": \"/output/joined-document.pdf\"}
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Merger Cloud also offers individual document merger SDKs for other languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_merger-for-net.webp"
          product: "GroupDocs.Merger"
          platform: ".NET"
          link: "/merger/net"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_merger-for-java.webp"
          product: "GroupDocs.Merger"
          platform: "Java"
          link: "/merger/java"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_merger-for-php.webp"
          product: "GroupDocs.Merger"
          platform: "PHP"
          link: "/merger/php"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_merger-for-python.webp"
          product: "GroupDocs.Merger"
          platform: "Python"
          link: "/merger/python"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_merger-for-ruby.webp"
          product: "GroupDocs.Merger"
          platform: "Ruby"
          link: "/merger/ruby"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_merger-for-node.webp"
          product: "GroupDocs.Merger"
          platform: "Node.js"
          link: "/merger/nodejs"
        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_merger-for-android.webp"
          product: "GroupDocs.Merger"
          platform: "Android"
          link: "/merger/android"
        

############################# Back to top ###############################
back_to_top:
  enable: true
---