---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Comparison"
product_tag: "comparison"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Comparison Cloud SDK for PDF Word Excel HTML Images"
head_description: "Java Cloud SDK for documents comparison. Use REST APIs to check content differences in PDF, Word, Excel, PPTX, Visio, Project, HTML & email file formats."

############################# Header ############################
title: "Java Cloud SDK to Compare Documents"
description: "Integrate document difference checker into your Java applications using REST API. Compare images, documents, eBooks, CAD & PDF files etc."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Comparison Cloud SDK for Java"
        image: "/sdk/272x272/groupdocs_comparison-for-java.webp"
        product: "GroupDocs.Comparison"
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
      GroupDocs.Comparison for Cloud is a REST API that enables your Java applications to compare two ‎same format documents to find differences between them make a resultant file and allow you to ‎accept or reject the retrieved changes. Our Document Comparison SDK for Java allows easy integration ‎into your existing applications, so that your end-users can compare documents, spreadsheets, ‎presentations, Microsoft Visio diagrams, emails, and files of many other formats.‎‎
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
        content: "Upload Documents to Cloud Storage and make Comparison"

      # feature loop
      - icon: "fas fa-desktop"
        content: "Retrieve Documents of Supported Formats for Comparison as File or Array of Images"

      # feature loop
      - icon: "fas fa-copy"
        content: "Based on Compared Documents Fetch Differences between Both in Resultant Document"
      
      # feature loop
      - icon: "fas fa-bullseye"
        content: "Get List of Categories, such as, TypeChanged or OnlyNumbers etc., for the Changed Content"

      # feature loop
      - icon: "fas fa-plug"
        content: "Accept or Reject the Changes to Save or Discard them"
      # feature loop
      - icon: "fas fa-file-o"
        content: "Return Updated Changes of the Resultant Document as a Set of Images or their Stream"
      # feature loop
      - icon: "fas fa-desktop"
        content: "Fetch Resultant Document (with updated changes) via Stream"
      # feature loop
      - icon: "fas fa-copy"
        content: "Get Document (with the result of comparison) as a Set of Images or their Stream"
      # feature loop
      - icon: "fas fa-bullseye"
        content: "Retrieve Resultant Document (with the Result of Comparison) as a Stream"
        
    more_feature:
      # more_feature_loop
      - title: "Get Changes from Compared Documents"
        content: "Using GroupDocs.Comparison Cloud API, you can compare documents and get list of changes, with just a few lines of code."

      # more_feature_loop
      - title: "Get changes from compared documents - cURL"
        content: |
      
          
          ```Java
          # TODO: Get your AppSID and AppKey at https://dashboard.groupdocs.cloud/#/apps (free registration is required).
          # For complete examples and data files, please go to https://github.com/groupdocs-comparison-cloud/groupdocs-comparison-cloud-java

          String  outPath = "result.docx",
          sourceName = "source.docx",
          targetName = "target.docx";

          StorageApi storageApi = Utils.getStorageApiInstance();

          // Upload files to Cloud Storage
          File file = new File("src/main/resources/" + sourceName);
          ResponseMessage storageresponse = storageApi.PutCreate("comparison/" + sourceName, null, null, file);
          file = new File("src/main/resources/" + targetName);
          storageresponse = storageApi.PutCreate("comparison/" + targetName, null, null, file);

          ChangesApi changesApi = Utils.getChangesApiInstance();
          PutChangesDocumentRequest request = new PutChangesDocumentRequest();
          request.setRequest(GetComparisonRequest(sourceName, targetName));
          request.setOutPath(outPath);
          Link response = changesApi.putChangesDocument(request);
          System.out.println(response);
          ```
      

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