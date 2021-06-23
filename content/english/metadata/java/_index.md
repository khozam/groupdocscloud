---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Metadata"
product_tag: "metadata"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Metadata Cloud SDK – Read Edit Remove Metadata from documents"
head_description: "Java metadata API to view, read, edit, analyze, find, delete, compare & export metadata of PDF Word Excel PPTX Outlook Visio Audio Video & Image documents."

############################# Header ############################
title: "Metadata Management Cloud SDK for Java"
description: "Metadata manipulation REST API to manage metadata properties from over 60 document, images and multimedia file formats in any language or platform.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Metadata Cloud SDK for Java"
        image: "/sdk/272x272/groupdocs_metadata-for-java.webp"
        product: "GroupDocs.Metadata"
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
            - link: "https://docs.groupdocs.cloud/metadatacloud/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-metadata-cloud/groupdocs-metadata-cloud-java"
        link_learn: "https://docs.groupdocs.cloud/metadatacloud/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Metadata Cloud SDK for Java makes it easier for developers to incorporate document metadata manipulation features within any java-based application by quickly integrating it with GroupDocs.Metadata Cloud REST API.

      The metadata extraction API is flexible and feature-rich, allowing users to view, add, update, search, retrieve and remove metadata properties from various document and image file formats such as Microsoft Office (Word, Excel, PowerPoint, Outlook, Visio, OneNote, and Project), PDF, metafiles, Photoshop and AutoCAD, audio and video file types. GroupDocs.Watermark Cloud is a REST API that can be used with any language or platform of your choice. It saves you valuable development cost and time by managing API requests and responses to let you focus only on writing up the specific source code that is needed in your project.


    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Metadata Cloud SDK for Java requires Java Runtime Environment and can run on any platform where these requirements can be met.

        
      
        right:
          enable: true
          icon: "fab fa-cubes"
          title: "Java Runtime Environment"
          content: |
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Metadata Cloud supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOT, DOTX, DOCM
                * **Excel:**  XLS, XLSX, XLSM, XLTM
                * **PowerPoint:** PPT, PPTX, POTM, POTX, PPTM, PPS, PPSX‎, PPSM‎
                * **Outlook:** MSG, EML
                * **OneNote:** ONE
                * **Visio:** VSD, VDX, VSDX, VSS, VSX
                * **Project:** MPP

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, ODS
                * **Portable**: PDF
                * **Photoshop**: PSD
                * **AutoCAD**: DWG, DXF
                * **Audio**: MP3, WAV
                * **Video**: AVI, MOV, QT, FLV
                * **Metafiles**: EMF, WMF
                * **vCard**: VCF‎, VCR
                * **Image**: JPG, JPEG, JPE, JP2, PNG, GIF, TIFF, WebP, BMP, DJVU, DJV, DICOM‎  
                * **OpenType Fonts**: OTF, OTC, TTF, TTC‎
                * **Others**: EPUB, ZIP, TORRENT, ASF

      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Metadata REST API while using your favorite language & platform.
        
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
    title: "Advanced Document Metadata REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Secured REST oriented Metadata Management API"

      # feature loop
      - icon: "fab fa-html5"
        content: "Supporting more than 60 popular file formats"

      # feature loop
      - icon: "fas fa-file-image"
        content: "Ability to View/Add Metadata"
      
      # feature loop
      - icon: "fas fa-file-alt"
        content: "Retrieve & Remove Metadata from Documents and Images"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Perform Search & Modify Metadata Operations on Supported File Types"

      # feature loop
      - icon: "fas fa-folder"
        content: "Flexible and Easy to Integrate with any language or platform"

      

    more_feature:
      # more_feature_loop
      - title: "Remove Metadata by Property Name - Java"
        content: |
          
          
          ```shell
            //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
            String MyAppKey = ""; // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
            String MyAppSid = ""; // Get AppKey and AppSID from https://dashboard.groupdocs.cloud
              
            Configuration configuration = new Configuration(MyAppSid, MyAppKey);
            MetadataApi apiInstance = new MetadataApi(configuration);
            
            RemoveOptions options = new RemoveOptions();
            SearchCriteria searchCriteria = new SearchCriteria();
            NameOptions nameOptions = new NameOptions();
            nameOptions.setValue("Application");
            searchCriteria.setNameOptions(nameOptions);
            options.setSearchCriteria(searchCriteria);
            FileInfo fileInfo = new FileInfo();
            fileInfo.setFilePath("documents/input.docx");
            options.setFileInfo(fileInfo);
            RemoveRequest request = new RemoveRequest(options);
            
            RemoveResult response = apiInstance.remove(request);
          ```
      # more_feature_loop
      - title: "Retrieve Hidden Data for Manipulation"
        content: |
          GroupDocs.Metadata for Java provides you a comprehensive way to get and delete hidden data from Microsoft Word, Excel and PowerPoint files. You can also do the same for PDF documents. Following list elaborates the sort of metadata you can access and manipulate through GroupDocs.Metadata for Java:  

          * Microsoft Word (Comments, Hidden Text, Merge Fields)
          * Microsoft Excel (Comments, Hidden Sheets)
          * Microsoft PowerPoint (Comments, Hidden Slides)
          * PDF Documents (Attachments, Annotations, Bookmarks, Form Fields)

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Metadata offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Metadata for cURL"
          image: "/sdk/272x272/groupdocs_metadata-for-curl.webp"
          product: "GroupDocs.Metadata"
          platform: "cURL"
          link: "/metadata/curl/"

        # solution loop
        - img_alt: "GroupDocs.Metadata for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-metadata-net.webp"
          product: "GroupDocs.Metadata"
          platform: ".NET"
          link: "/metadata/net/"

        # solution loop
        - img_alt: "GroupDocs.Metadata for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-metadata-java.webp"
          product: "GroupDocs.Metadata"
          platform: "Java"
          link: "/metadata/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---