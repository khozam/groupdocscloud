---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Classification"
product_tag: "classification"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Documents & Text Classification Cloud SDK for PDF Word Text"
head_description: "Document and raw text classification with c# .NET APIs. Categorization with IAB-2 and Documents taxonomies and consumer sentiment analysis with a taxonomy Sentiment."

############################# Header ############################
title: "Classify Documents & Text with .NET SDK"
description: "‎‎.NET Cloud SDK to communicate with classification REST API for automated classification of text and documents according to IAB-2, Documents, or Sentiment taxonomy.‎‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Classification for Cloud"
        image: "/sdk/272x272/groupdocs_classification-for-net.webp"
        product: "GroupDocs.Classification"
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
            - link: "https://docs.groupdocs.cloud/classification/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/classification/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Classification Cloud SDK for .NET enables you to classify your raw text as well as documents ‎into predefined categories. Classification Cloud SDK supports multiple taxonomy types, such as IAB-2, Documents & Sentiment taxonomy. Classification information can be viewed regarding classes as well ‎as their respective probabilities.‎
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Classification Cloud SDK for .NET.
      
        right:
          enable: true
          icon: "fas fa-object-group"
          title: "Overview"
          content: |
            * Classify Raw Data
            * Classify Document
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Classification Cloud SDK for .NET supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF‎
                
        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT
                * **Fixed Layout**:  PDF
                * **Text**: TXT
                

        


      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Classification Cloud SDK for .NET - some of the supported languages and platforms.
      
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
    title: "Advanced Document Classification REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-filter"
        content: "Classify raw text based on IAB-2, Documents, and Sentiment taxonomies"

      # feature loop
      - icon: "fas fa-check-square"
        content: "Perform classification of the documents as per IAB-2, Documents, or Sentiment taxonomies"

      # feature loop
      - icon: "fas fa-eye"
        content: "View classification information regarding classes and their respective probabilities"
      
      # feature loop
      - icon: "fas fa-bolt"
        content: "Speed up the development process"

      # feature loop
      - icon: "fas fa-folder"
        content: "100% tested and out of the box running"

      # feature loop
      - icon: "fas fa-thumbs-up"
        content: "Convenient to use API"

      # feature loop
      - icon: "fas fa-smile"
        content: "Easy integration with REST API"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"

      # feature loop
      - icon: "fas fa-list-alt"
        content: "API explorer based on swagger collection"
      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"
      # feature loop
      - icon: "fas fa-list"
        content: "API explorer based on swagger collection"
    
    more_feature:
      # more_feature_loop
      - title: "Supported Types of Taxonomy"
        content: "GroupDocs.Classification Cloud SDK for .NET performs classification based on four types of Taxonomies. The raw text or document classification is done as per IAB-2, Document, Sentiment, or Sentiment3 taxonomies. Following example shows how to classify raw text based on IAB-2 taxonomy using SDK:‎‎"

      # more_feature_loop
      - title: "Get document page as responsive HTML - .NET"
        content: |
          
          
          ```cs
          var request = new ClassifyRequest(new BaseRequest()
            {
              Description = "Try Text classification"
            },
            "3");
          // Get classification results
          var response = apiInstance.Classify(request);
          Debug.Print(response.ToString());
          ```
      
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Viewer Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_translation-for-curl.webp"
          product: "GroupDocs.Viewer"
          platform: "cURL"
          link: "/classification/curl/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_translation-for-net.webp"
          product: "GroupDocs.Viewer"
          platform: ".NET"
          link: "/classification/net/"

      

     

        

############################# Back to top ###############################
back_to_top:
  enable: true
---