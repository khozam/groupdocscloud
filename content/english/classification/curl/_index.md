---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Classification"
product_tag: "classification"
platform: "cURL"
platform_tag: "curl"

############################# Head ############################
head_title: "Documents & Text Classification in Cloud | cURL for REST API"
head_description: "REST API to classify raw text from PDF, Microsoft Word, OpenDocument & rich text documents via cURL commands as per IAB-2 taxonomy."

############################# Header ############################
title: "Text & Document Classification with cURL"
description: "Classify raw text and documents as per IAB-2, Documents, and Sentiment taxonomy into predefined classes."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Classification for Cloud"
        image: "/sdk/272x272/groupdocs_classification-for-curl.webp"
        product: "GroupDocs.Classification"
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
      GroupDocs.Classification Cloud for cURL provides you an automated way to classify your raw text or documents into ‎predefined categories based on IAB-2, Documents, or Sentiment taxonomy.‎ 
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the main features supported by GroupDocs.Classification Cloud for cURL.
      
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
          GroupDocs.Classification Cloud for cURL supports a number of document formats.

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
          GroupDocs.Classification Cloud for cURL - some of the supported languages and platforms.
      
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
      - icon: "fas fa-random"
        content: "Classification of pivot tables in Excel workbooks"
      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"
      # feature loop
      - icon: "fas fa-list"
        content: "API explorer based on swagger collection"
    
    more_feature:
      # more_feature_loop
      - title: "Supported Types of Taxonomy"
        content: "GroupDocs.Classification Cloud SDK for .NET performs classification based on three types of Taxonomies. ‎The raw text or document classification is done as per IAB-2, Document, or Sentiment ‎taxonomies. Following example shows how to classify raw text based on IAB-2 taxonomy using cURL:‎‎"

      # more_feature_loop
      - title: "Raw Text Classification as per IAB-2 Taxonomy - cURL - Request"
        content: |
          
          
          ```shell
          curl -X POST "https://api.groupdocs.cloud/v1.0/classification/classify?BestClassesCount=3" \
          -H "accept: application/json" \
          -H "authorization: Bearer TOKEN" \
          -H "Content-Type: application/json" \
          -d "{ \"description\": \"Medicine is an important part of our life\"}"
          ```
      # more_feature_loop
      - title: "Raw Text Online Classification as per IAB-2 Taxonomy - cURL - Response"
        content: |
          
          
          ```shell
              {
              "bestClassName": "Healthy_Living",
              "bestClassProbability": 53.77,
              "bestResults": [
                  {
                      "className": "Healthy_Living",
                      "classProbability": 53.77
                  },
                  {
                      "className": "Medical_Health",
                      "classProbability": 38.27
                  },
                  {
                      "className": "Pets",
                      "classProbability": 1.98
                  }
              ],
              "code": 200,
              "status": "OK"
          }
          
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
          platform: " .NET"
          link: "/classification/net/"

      

     

        

############################# Back to top ###############################
back_to_top:
  enable: true
---