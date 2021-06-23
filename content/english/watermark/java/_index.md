---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Cloud Watermark Management SDK for PDF Word Excel Diagrams PPTX"
head_description: "Java document watermarking API – Generate, search & remove watermarks from documents: PDF, Word, Excel, presentations, Visio, email and image file formats."

############################# Header ############################
title: "Java Cloud SDK for Document Watermarking"
description: "Add, edit, search and delete watermarks from all popular document and images file formats using watermarking Cloud SDK for Java and REST API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "Java Document Watermark SDK"
        image: "/sdk/272x272/groupdocs_watermark-for-java.webp"
        product: "GroupDocs.Watermark"
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
            - link: "https://wiki.groupdocs.cloud/watermarkcloud/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-watermark-cloud/groupdocs-watermark-cloud-java"
        link_learn: "https://docs.groupdocs.cloud/watermarkcloud/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      The API is flexible, feature-rich and offers straightforward methods to manage and manipulate watermarks from supported document types. Perform watermarking features like adding, searching, updating and deleting without using any external software. The watermarking SDK is makes it possible to perform watermark search operation within documents and edit or remove watermarks that were added already by any third-party tool. You can also control the customization of watermarks by specifying the text style, font, size, color or position as per your project requirements.

      GroupDocs.Watermark Cloud is a REST API that makes it a perfect choice for programmers to use it with any language or platform that is capable to make REST API calls. It easily integrates with other cloud services to provide an optimal watermarks management experience across web, mobile desktop or cloud platforms.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Watermark Cloud SDK for Java has following SDK Requirements:

        right:
          enable: true
          icon: "fab fa-cubes"
          title: "Java Runtime Environment"
          content: |
            


        
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Watermark Cloud SDK for Java supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel:** XLS, XLSX, XLT, XLSM, XLTX, XLTM
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, PPTM, POTX, POTM
                * **Visio:** VSD, VSDX, VSDM, VSTX, VSTM, VSS, VSSX, VSSM, VDX, VSX, VTX

            
                

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT
                * **Fixed Layout**: PDF
                * **Image Files**: BMP, GIF, JPG, JPEG, JP2, PNG, TIFF, WebP
                * **Other**: RTF

            

      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Watermark REST API while using your favorite language & platform.
        
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
    title: "Advanced watermark management API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Secured watermark management solution"

      # feature loop
      - icon: "fas fa-file-image"
        content: "Add or Remove Watermark from a specific pages or whole document"

      # feature loop
      - icon: "fas fa-file-alt"
        content: "Find text or image-based watermarks inside the documents"
      
      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Manage formatting settings to manipulate watermarks"

      # feature loop
      - icon: "fas fa-folder"
        content: "Cloud REST API to be used with any language or platform"

      # feature loop
      - icon: "fas fa-lock"
        content: "Search and delete already added watermarks from supported file formats"

      
    more_feature:
      # more_feature_loop
      - title: "Remove Watermark from Document – Java"
        content: |
          
          
          ```java
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
          public class RemoveWatermarks {

            public static void main(String[] args) {

              WatermarkApi apiInstance = new WatermarkApi(Common.GetConfiguration());

              try {
                FileInfo fileInfo = new FileInfo();
                fileInfo.setFilePath("with_watermarks/sample.pdf");
                fileInfo.setStorageName(Common.MyStorage);
                RemoveOptions options = new RemoveOptions();
                options.setFileInfo(fileInfo);
                
                ImageSearchCriteria imageSearchCriteria = new ImageSearchCriteria();
                FileInfo imageFileInfo = new FileInfo();
                imageFileInfo.setFilePath("watermark_images/sample_watermark.webp");
                imageFileInfo.setStorageName(Common.MyStorage);
                imageSearchCriteria.setImageFileInfo(imageFileInfo);
                options.setImageSearchCriteria(imageSearchCriteria);
                
                TextSearchCriteria textSearchCriteria = new TextSearchCriteria();
                textSearchCriteria.setSearchText("Watermark text");
                options.setTextSearchCriteria(textSearchCriteria);
                
                options.setOutputFolder("removed_watermarks");
                
                RemoveRequest request = new RemoveRequest(options);
                RemoveResult response = apiInstance.remove(request);

                System.out.println("Resultant file path: " + response.getPath());
              } catch (ApiException e) {
                System.err.println("Exception while calling WatermarkApi:");
                e.printStackTrace();
              }
            }
          }
          
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Watermark offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Watermark for cURL"
          image: "/sdk/272x272/groupdocs_watermark-for-curl.webp"
          product: "GroupDocs.Watermark"
          platform: "cURL"
          link: "/watermark/curl/"

        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/sdk/272x272/groupdocs_watermark-for-net.webp"
          product: "GroupDocs.Watermark"
          platform: ".NET"
          link: "/watermark/net/"
        
        # solution loop
        - img_alt: "GroupDocs.Watermark for .NET"
          image: "/sdk/272x272/groupdocs_watermark-for-java.webp"
          product: "GroupDocs.Watermark"
          platform: "Java"
          link: "/watermark/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---