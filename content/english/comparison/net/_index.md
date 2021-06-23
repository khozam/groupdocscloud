---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Comparison"
product_tag: "comparison"
platform: ".NET"
platform_tag: ".net"

############################# Head ############################
head_title: ".NET Document Comparison Cloud SDK for PDF Word Excel HTML Images"
head_description: ".NET Cloud SDK for documents comparison to check content differences. Use REST APIs to compare PDF, Word, Excel, PPTX, Outlook, HTML and images."

############################# Header ############################
title: "Comparing Documents via C# .NET SDK"
description: "Develop .NET based business document comparison tools using Cloud API with support to check difference among files of all popular formats."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Comparison Cloud SDK for .NET"
        image: "/sdk/272x272/groupdocs_comparison-for-net.webp"
        product: "GroupDocs.Comparison"
        platform: ".NET"

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
      GroupDocs.Comparison Cloud API provides a one-stop-shop solution for comparing documents in all common business formats. Supported file types include PDF, Microsoft Word documents, Excel spreadsheets, PowerPoint presentations, plain text, and others.‎
      Our API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming, therefore, we have provided and supports SDKs in many development languages in order to make it easier to integrate with our Cloud Comparison services. If you use our SDK for .NET, it will hide the REST API calls and will let you use GroupDocs.Comparison Cloud API features in a native way for your .NET application.
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
        content: "Using SDK for .NET for GroupDocs.Comparison Cloud API, you can compare documents and get the list of changes, with just a few lines of code."

      # more_feature_loop
      - title: "Get changes from compared documents - C#"
        content: |
          
          
          ```.NET
          //Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
            var configuration = new Configuration {AppSid = Sid, AppKey = Key};
            var apiInstance = new ChangesApi();
            var request = new ComparisonRequest(); // ComparisonRequest | The request. (optional) 
            // Posts the categories changes.
            List result = apiInstance.PostCategoriesChanges(request, categoriesType);
            Debug.WriteLine(result);
            ```
      # more_feature_loop
      - title: "Accurate Content Comparison"
        content: "Irrespective of the file format, GroupDocs.Comparison Cloud API is able to identify changes in literally all document elements, including texts, lines, boxes, margins, etc. This allows users to get complete details of all changes made to the document: texts, font types and styles, page headers, footers, and overall layout – all are precisely analyzed and reported when differences are found."

      # more_feature_loop
      - title: "Advanced Document Handling"
        content: "GroupDocs.Comparison Cloud provides two main resources (Document and Changes) which allows retrieving compared documents (as file or array of images) or its changes. Also, it provides the ability to update (accept or reject) retrieved changes."
      # more_feature_loop
      - title: "Easy Customization"
        content: "GroupDocs.Comparison Cloud SDK for .NET is 100% tested and out of the box running. The SDK is open source and has an MIT license. You can use it, and even customize it for absolutely free of charge."
      

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
        - img_alt: "GroupDocs.Comparison Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_comparison-for-java.webp"
          product: "GroupDocs.Comparison"
          platform: "Java"
          link: "/comparison/java"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_comparison-for-php.webp"
          product: "GroupDocs.Comparison"
          platform: "PHP"
          link: "/comparison/php"

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