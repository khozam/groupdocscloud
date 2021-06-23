---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Merger"
product_tag: "merger"
platform: "Nodejs"
platform_tag: "nodejs"

############################# Head ############################
head_title: "Node.js Cloud SDK to Merge & Split PDF Word Excel Diagrams HTML Documents"
head_description: "Node.js cloud document merger SDK & REST API to merge & split pages of PDF, Word, Excel, diagrams & HTML file formats."

############################# Header ############################
title: "Node.js SDK for Documents Merging & Splitting"
description: "Enhance capabilities of your tools and applications with advanced document merging and splitting features using REST API & Node.js Cloud SDK."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Merger Cloud SDK for Nodejs"
        image: "/sdk/272x272/groupdocs_merger-for-node.webp"
        product: "GroupDocs.Merger"
        platform: "Node.js"

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
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-merger-cloud-node"
        link_learn: "https://docs.groupdocs.cloud/merger/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Merger Cloud SDK for Node.js is a robust solution to combine, split, remove and rearrange single page or a collection of pages from various document formats. Representing the document pages as images is one many useful features to quickly analyse the content and document structure. It supports working with a wide range of document formats including Microsoft Office Word, Excel spreadsheets, PowerPoint presentations, Visio drawings, OneNote, PDF, HTML, OpenDocument, text and many others.
      Extract basic information of the document and perform document security operations by applying updating or deleting password protections from supported document formats. The API is also helpful to extract, swap or rotate selected pages from the source document and accurately generates a new resultant document based on specified pages from the source document.
      GroupDocs.Merger Cloud SDK for Node.js is built as a layer on top of GroupDocs.Merger Cloud REST API that can be used with any language or development platform that can call REST APIs.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document merger Cloud API for Node.js.
      
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
      - title: "Join pages from various documents - Node.js"
        content: |
          
          ```Node.js
            //Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).
            class JoinPagesFromVariousDocuments {
            static async Run() {
            
              let item1 = new merger_cloud.JoinItem();
              item1.fileInfo = new merger_cloud.FileInfo();
              item1.fileInfo.filePath = "WordProcessing/sample-10-pages.docx";
              item1.pages = [3, 6, 8];

              let item2 = new merger_cloud.JoinItem();
              item2.fileInfo = new merger_cloud.FileInfo();
              item2.fileInfo.filePath = "WordProcessing/four-pages.docx";
              item2.startPageNumber = 1
              item2.endPageNumber = 4
              item2.rangeMode = merger_cloud.JoinItem.RangeModeEnum.OddPages;
                
              let options = new merger_cloud.JoinOptions();
              options.joinItems = [item1, item2];
              options.outputPath = "Output/joined-pages.docx";

              let result = await documentApi.join(new merger_cloud.JoinRequest(options));

              console.log("Output file path: " + result.path);
            }
          }
          module.exports = JoinPagesFromVariousDocuments;
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
        - img_alt: "GroupDocs.Merger Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_merger-for-android.webp"
          product: "GroupDocs.Merger"
          platform: "Android"
          link: "/merger/android"
        

############################# Back to top ###############################
back_to_top:
  enable: true
---