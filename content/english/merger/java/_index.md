---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Merger"
product_tag: "merger"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Cloud SDK | Merger Cloud API | Split &amp; Merge Documents"
head_description: "Documents merging API for Java. Merge, split, swap, reorder and delete pages of PDF, Microsoft Word, Excel, presentations, Visio, XPS &amp; EPUB formats."

############################# Header ############################
title: "Split and Merge Documents with Java SDK"
description: "Java SDK as a wrapper for the GroupDocs.Merger Cloud API. Combine documents into one, split document into many in your Java applications."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Merger Cloud SDK for Java"
        image: "/sdk/272x272/groupdocs_merger-for-java.webp"
        product: "GroupDocs.Merger"
        platform: "Java"

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
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-merger-cloud-java"
        link_learn: "https://docs.groupdocs.cloud/merger/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Merger Cloud SDK for Java is a wrapper to communicate with the Cloud API for Java developers. The GroupDocs.Merger Cloud API is a REST service to merge and split documents and supports a wide range of Microsoft Office, OpenDocument, eBook, PDF, text, LaTeX and other document formats.
      The GroupDocs.Merger Cloud API provides a way to combine two or more documents into one, split any document to many, and generate image representation of any document in PNG, JPG to BMP format. The API offers many other document pages related operations like rotate any page of a PDF document, swap slides of presentations or change page orientation of word documents. The API gives importance to security and allows to apply or remove the password protection to your important business documents.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document merger Cloud API for Java.
      
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
            * Combine multiple documents into on
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
      - title: "Merge multiple documents"
        content: "Using GroupDocs.Merger Cloud API, you can combine two or more documents into one, or split any document into multiple smaller documents. Following few lines of code shows how to combine two word files in Java."

      # more_feature_loop
      - title: "Merge word documents - Java"
        content: |
          
          ```java
            //Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).
            Configuration configuration = new Configuration(MyAppSid, MyAppKey);
            DocumentApi apiInstance = new DocumentApi(configuration);
      
            FileInfo fileInfo1 = new FileInfo();         
            fileInfo1.setFilePath("foldername/doc1.docx");
            JoinItem item1 = new JoinItem();
            item1.setFileInfo(fileInfo1);
      
            FileInfo fileInfo2 = new FileInfo();            
            fileInfo2.setFilePath("foldername/doc2.docx");
            JoinItem item2 = new JoinItem();
            item2.setFileInfo(fileInfo2);
      
            JoinOptions options = new JoinOptions();
            options.setJoinItems(Arrays.asList(item1, item2));
            options.setOutputPath("output/mergedDoc.docx");
      
            JoinRequest request = new JoinRequest(options);
            DocumentResult response = apiInstance.join(request);			
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