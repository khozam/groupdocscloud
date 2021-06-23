---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Viewer"
product_tag: "viewer"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Viewing Cloud SDK | Render PDF Word Excel Visio HTML"
head_description: "Work with Java document viewer Cloud SDK & REST APIs to create tools for rendering Word, Excel spreadsheet, PDF, PPTX, HTML, images, emails etc."

############################# Header ############################
title: "Document Viewing REST API & Java Cloud SDK"
description: "Build robust document rendering & viewing tools using Java REST API. Boost your development without worrying about underlying details.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Viewer Cloud SDK for Java"
        image: "/sdk/272x272/groupdocs_viewer-for-java.webp"
        product: "GroupDocs.Viewer"
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
            - link: "https://docs.groupdocs.cloud/viewer/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-viewer-cloud/groupdocs-viewer-cloud-java"
        link_learn: "https://github.com/groupdocs-viewer-cloud/groupdocs-viewer-cloud-java"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Viewer Cloud is a true REST API that gives the complete freedom of platform & programming language whereas GroupDocs.Viewer Cloud SDK for Java is built as a layer on the top of GroupDocs.Viewer Cloud REST API, allowing a higher level of abstraction so that you don't need to know the REST API to use this SDK.

      GroupDocs.Viewer Cloud API allows you to seamlessly enhance your application with the capability to render a number of document formats with the ability to view a specific document in HTML, image, PDF or its original format. You also get the flexibility to render the whole document, page by page or custom range of pages. GroupDocs.Viewer Cloud SDK for Java has been developed to help you integrate all these features in your Java application without any hassle.


    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Viewer Cloud SDK for Java requires Java Runtime Environment and can run on any platform where these requirements can be 

        right:
          enable: true
          icon: "fas fa-cubes"
          title: "Java Runtime Environment"
          content: |
            
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Viewer Cloud SDK for Java supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTX, XLTM
                * **PowerPoint:**  PPT, PPTX, PPS, PPSX, PPSM, PPTM, POTX, POTM
                * **Visio:** VSD, VSDX, VSDM, VST, VSTX, VSTM, VSS, VSSX, VSSM, VDX, VSX, VTX, VDW
                * **Project:** MPP, MPT
                * **Outlook:** MSG, EML, PST, OST
                * **OneNote:** ONE

            

        right:
          enable: true
          table:
            # table loop
            - title: "Images, Graphics & Diagrams"
              content: |
                * **OpenDocument:** ODT, OTT, ODS, OTS, ODP, OTP, ODG
                * **Fixed Layout:** PDF, XPS
                * **eBook:** EPUB, MOBI
                * **Image Files:** BMP, GIF, ICO, JPG, JPEG, PNG, PSD, SVG, TIF, TIFF, Webp, DjVu, DNG, DCM (DICOM)
                * **JPEG2000:** JP2, J2C, J2K, JPF, JPX, JPM
                * **CAD:** DGN, DWF, DWG, DXF, IFC, STL
                * **Markup:** HTML, MHT, MHTML, XML
                * **Metafile:** WMF, EMF, CGM
                * **Apple Mail:** EMLX
                * **PostScript:** PS, EPS
                * **Other:** RTF, TXT, TEX, CSV, TSV, PCL
                
      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Viewer Cloud for cURL - some of the supported languages and platforms.
        
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
    title: "Advanced Document Viewer REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Render documents as HTML5"

      # feature loop
      - icon: "fas fa-images"
        content: "Render documents as Image"

      # feature loop
      - icon: "fas fa-file-alt"
        content: "Rotate, reorder & watermark pages"
      
      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render documents as PDF"

      # feature loop
      - icon: "fas fa-paperclip"
        content: "Render document attachments"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"

     

      

    more_feature:
      # more_feature_loop
      - title: "Quick Files and Folder List from the Storage"
        content: |
          The cloud-based viewer API can quickly provide the complete list of existing files and folders with few lines of code.
          
          Get Files List from the Specific Storage and Folder - Java
          
          ```java
          //Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).

          FolderApi apiInstance = new FolderApi(appSID, appKey);
          GetFilesListRequest request = new GetFilesListRequest("folder name", "storage name");
          FilesList response = apiInstance.getFilesList(request);
          for (StorageFile storageFile : response.getValue()) {
          System.out.println((storageFile.getIsFolder() ? "Folder - " : "File - ") + storageFile.getPath());
          }
          ```
      # more_feature_loop
      - title: "Quickly Get Started with Document Viewing REST API"
        content: "Get started quickly using GroupDocs.Viewer Cloud REST API with the GroupDocs.Viewer Cloud SDK for Java. It facilitates the users and speeds up the development of their applications written in Java while taking care of a lot of low-level details of making requests and handling responses and lets the users focus on writing code specific to their particular project. "

      # more_feature_loop
      - title: "Easy Customization Options"
        content: "GroupDocs.Viewer Cloud SDK is 100% tested and out of the box running. The SDK is open source and has an MIT license. You can use it, and even customize it for absolutely free of charge."
       
       

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
          image: "/sdk/272x272/groupdocs_viewer-for-curl.webp"
          product: "GroupDocs.Viewer"
          platform: "cURL"
          link: "/viewer/curl/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_viewer-for-net.webp"
          product: "GroupDocs.Viewer"
          platform: ".NET"
          link: "/viewer/net/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_viewer-for-java.webp"
          product: "GroupDocs.Viewer"
          platform: "Java"
          link: "/viewer/java/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_viewer-for-php.webp"
          product: "GroupDocs.Viewer"
          platform: "PHP"
          link: "/viewer/php/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_viewer-for-python.webp"
          product: "GroupDocs.Viewer"
          platform: "Python"
          link: "/viewer/python/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_viewer-for-ruby.webp"
          product: "GroupDocs.Viewer"
          platform: "Ruby"
          link: "/viewer/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_viewer-for-node.webp"
          product: "GroupDocs.Viewer"
          platform: "Node.js"
          link: "/viewer/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_viewer-for-android.webp"
          product: "GroupDocs.Viewer"
          platform: "Android"
          link: "/viewer/android/"
    

############################# Back to top ###############################
back_to_top:
  enable: true
---