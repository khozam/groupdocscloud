---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Merger"
product_tag: "merger"
platform: "Python"
platform_tag: "python"

############################# Head ############################
head_title: "Python Cloud SDK to Merge &amp; Split PDF Word Excel Diagrams HTML Documents"
head_description: "Python cloud document merger SDK and REST API to merge, combine and split pages of PDF, Word, Excel, diagrams &amp; HTML file formats."

############################# Header ############################
title: "Join & Split Documents with Python SDK"
description: "Cloud REST API to join, swap, trim, split or move documents, spreadsheets, presentations, PDF and OpenDocument file formats within Python applications."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Merger Cloud SDK for Python"
        image: "/sdk/272x272/groupdocs_merger-for-python.webp"
        product: "GroupDocs.Merger"
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
            - link: "https://docs.groupdocs.cloud/merger/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-merger-cloud-python"
        link_learn: "https://docs.groupdocs.cloud/merger/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Merger Cloud SDK for Python is a flexible document merging and splitting solution for a bunch of popular document formats including Microsoft Office Word, Excel, PowerPoint, Visio, OneNote, PDF, HTML, OpenDocument, text and many others.
      The Merger API provides a convenient solution to combine two or more documents into a single document or split up one source document into multiple resultant documents. You can also preview the document pages as images for the whole document or choosing the preferred page range according to the customized document previewing requirements. The SDK also support performing document operations to shift, delete, exchange, rotate or change the page orientation either as portrait or landscape for whole or preferred range of pages.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document merger Cloud API for Python.
      
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
          Document merger Cloud API for Java supported formats.

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
      - title: "Preview document pages as image - Python"
        content: |
          
          ```Python
            //Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).
            class PreviewDocument:
            @classmethod
            def Run(cls):
              documentApi = groupdocs_merger_cloud.DocumentApi.from_keys(Common.app_sid, Common.app_key)
              
              options = groupdocs_merger_cloud.PreviewOptions()
              options.file_info = groupdocs_merger_cloud.FileInfo("WordProcessing/four-pages.docx")
              options.output_path = "Output/preview-page"
              options.pages = [1, 3]
              options.format = "Png"

              result = documentApi.preview(groupdocs_merger_cloud.PreviewRequest(options))        

              print("Documents count = " + str(len(result.documents)))							
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
        - img_alt: "GroupDocs.Merger Cloud for cURL"
          image: "/sdk/272x272/groupdocs_merger-for-curl.webp"
          product: "GroupDocs.Merger"
          platform: "Cloud for cURL"
          link: "/merger/curl"

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