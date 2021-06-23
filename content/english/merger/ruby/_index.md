---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Merger"
product_tag: "merger"
platform: "Ruby"
platform_tag: "ruby"

############################# Head ############################
head_title: "Ruby Cloud SDK to Merge & Split PDF Word Excel Diagrams HTML Documents"
head_description: "Ruby cloud document merger SDK &amp; REST API to merge &amp; split pages of PDF, Word, Excel, diagrams &amp; HTML file formats."

############################# Header ############################
title: "Combine & Split Documents with Ruby SDK"
description: "REST APIs & Ruby Cloud SDK to merge, split, shuffle or remove pages from popular document file formats."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Merger Cloud SDK for Ruby"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-ruby.png"
        product: "GroupDocs.Merger"
        platform: "Cloud SDK for Ruby"

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
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-merger-cloud-ruby"
        link_learn: "https://docs.groupdocs.cloud/merger/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      Build high performance business applications in Ruby to combine, split, shuffle, rotate or delete single page or whole document of the same format in your Ruby applications. The supported file types include PDF, MS Word, Excel spreadsheets, presentations, drawings, HTML and many others industry standard formats.
      Developers can easily perform document pages related operations like swapping, removing, extracting pages from source document to combine as a new resultant document and setting the page orientation to portrait or landscape mode. The API also offers optimized document security features to apply, update or remove passwords from the supported document formats.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document merger Cloud API for Ruby.
      
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
      - title: "Split to multiple page document - Ruby"
        content: |
          
          ```Ruby
            //Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).
            class SplitToMultiPageDocuments
            def self.Run()    
              documentApi = GroupDocsMergerCloud::DocumentApi.from_keys($app_sid, $app_key)
              options = GroupDocsMergerCloud::SplitOptions.new
              options.file_info = GroupDocsMergerCloud::FileInfo.new
              options.file_info.file_path = 'WordProcessing/sample-10-pages.docx'
              options.output_path = "Output/split-to-multipage-document"
              options.pages = [3, 6, 8]
              options.mode = "Intervals"

              result = documentApi.split(GroupDocsMergerCloud::SplitRequest.new(options))
            
              puts("Documents count: " + result.documents.size.to_s)
            end
          end
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
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-curl.png"
          product: "GroupDocs.Merger"
          platform: "Cloud for cURL"
          link: "/merger/curl"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-net.png"
          product: "GroupDocs.Merger"
          platform: "Cloud SKD for .NET"
          link: "/merger/net"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-java.png"
          product: "GroupDocs.Merger"
          platform: "Cloud SDK for Java"
          link: "/merger/java"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for PHP"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-php.png"
          product: "GroupDocs.Merger"
          platform: "Cloud SDK for PHP"
          link: "/merger/php"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Python"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-python.png"
          product: "GroupDocs.Merger"
          platform: "Cloud SDK for Python"
          link: "/merger/python"

        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Node.js"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-node.png"
          product: "GroupDocs.Merger"
          platform: "Cloud SDK for Node.js"
          link: "/merger/nodejs"
        # solution loop
        - img_alt: "GroupDocs.Merger Cloud SDK for Android"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_merger-for-android.png"
          product: "GroupDocs.Merger"
          platform: "Cloud SDK for Android"
          link: "/merger/android"
        

############################# Back to top ###############################
back_to_top:
  enable: true
---