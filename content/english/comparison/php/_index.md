---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Comparison"
product_tag: "comparison"
platform: "PHP"
platform_tag: "php"

############################# Head ############################
head_title: "PHP Document Comparison Cloud SDK for PDF Word Excel HTML & Images"
head_description: "PHP document comparison &amp; difference checker Cloud SDK. Use REST APIs to compare PDF, Word, Excel, Presentations, Outlook, HTML and images."

############################# Header ############################
title: "Compare Documents via PHP Cloud SDK"
description: "Build content comparison applications with PHP Cloud SDK for comparison REST API. Compare, find differences, accept or reject changes in files of popular formats."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Comparison Cloud SDK for PHP"
        image: "/sdk/272x272/groupdocs_comparison-for-php.webp"
        product: "GroupDocs.Comparison"
        platform: "PHP"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/comparison/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/comparison/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      Get started using GroupDocs.Comparison Cloud API features in your PHP applications with the help of our GroupDocs.Comparison Cloud SDK for PHP. It provides a one-stop-shop solution for comparing documents in all common business formats. Supported file types include PDF, Microsoft Word documents, Excel spreadsheets, PowerPoint presentations, plain text, and others.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document comparison Cloud API.
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fas fa-check"
              title: "Accept retrieved changes"
              
            # table loop
            - icon: "fas fa-bookmark-o"
              title: "Document Resources"
              content: |
                * Result document
                * Stream of result
                * Images of result

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-trash-o"
              title: "Reject retrieved changes"
              
            # table loop
            - icon: "fas fa-retweet"
              title: "Changes Resources"
              content: |
                * Get changes
                * Update changes

      ## TAB TWO ##
      tab_two:
        description: |
          Document comparison Cloud API supported formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOCM, DOTM, RTF
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLS2003
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Outlook**: EML, EMLX, MSG

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP
                * **Web**: HTM, HTML, MHTML
                        * **Fixed Layout**: PDF
                * **Image Files**: JPEG, BMP, PNG, GIF
                        * **Text**: TXT and other text formats with different extensions
                * **Others**: DJVU, DICOM, PDF, CSV


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
    title: "Advanced Document Comparison REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-file-o"
        content: "Multiple file formats support"

      # feature loop
      - icon: "fas fa-desktop"
        content: "Cross-platform compatibility"

      # feature loop
      - icon: "fas fa-copy"
        content: "Retrieve compared documents"
      
      # feature loop
      - icon: "fas fa-bullseye"
        content: "Accurate content comparison"

      # feature loop
      - icon: "fas fa-plug"
        content: "Accept or reject retrieved changes"
    
    more_feature:
      # more_feature_loop
      - title: "Get Changes from Compared Documents"
        content: "Using GroupDocs.Comparison Cloud API, you can compare documents and get the list of changes, with just a few lines of code."

      # more_feature_loop
      - title: "Get changes from compared documents - PHP"
        content: |
          
          
          ```PHP
          //Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
            $configuration = new Configuration();
            $configuration->setAppSid($sid);
            $configuration->setAppKey($key);
            $apiInstance = new ChangesApi($configuration);
            $comparisonRequest = new ComparisonRequest($sourceFile,$targetFiles,$settings,$changes);
            $request = new PostCategoriesChangesRequest($comparisonRequest,$catergoriesType);
            $response = $apiInstance->postCategoriesChanges($request);
            ```
      # more_feature_loop
      - title: "Accurate Content Comparison"
        content: "Irrespective of the file format, GroupDocs.Comparison Cloud API is able to identify changes in literally all document elements, including texts, lines, boxes, margins, etc. This allows users to get complete details of all changes made to the document: texts, font types and styles, page headers, footers, and overall layout – all are precisely analyzed and reported when differences are found."

      # more_feature_loop
      - title: "Advanced Document Handling"
        content: "GroupDocs.Comparison Cloud provides two main resources (Document and Changes) which allows retrieving compared documents (as file or array of images) or its changes. Also, it provides the ability to update (accept or reject) retrieved changes."
      # more_feature_loop
      - title: "SDK Benefits"
        content: "GroupDocs.Comparison Cloud API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API SDKs in many development languages in order to make it easier to integrate with us. If you use SDK, it hides the REST API calls and lets you use GroupDocs.Comparison Cloud API features in a native way for your preferred language."
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Comparison Cloud also offers individual document comparison SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_comparison-for-curl.webp"
          product: "GroupDocs.Comparison"
          platform: "Cloud for cURL"
          link: "/comparison/curl"
        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_comparison-for-net.webp"
          product: "GroupDocs.Comparison"
          platform: ".NET"
          link: "/comparison/net"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_comparison-for-java.webp"
          product: "GroupDocs.Comparison"
          platform: "Java"
          link: "/comparison/java"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_comparison-for-python.webp"
          product: "GroupDocs.Comparison"
          platform: "Python"
          link: "/comparison/python"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_comparison-for-ruby.webp"
          product: "GroupDocs.Comparison"
          platform: "Ruby"
          link: "/comparison/ruby"
        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_comparison-for-node.webp"
          product: "GroupDocs.Comparison"
          platform: "Node.js"
          link: "/comparison/nodejs"

        

############################# Back to top ###############################
back_to_top:
  enable: true
---