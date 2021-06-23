---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Watermark"
product_tag: "watermark"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Cloud Watermark Management SDK for PDF Word Excel Diagrams PPTX"
head_description: "C# .NET API to add, search and remove image & text-based watermarks from documents: PDF, Word, Excel, presentations, Visio, email and image file formats."

############################# Header ############################
title: ".NET Cloud SDK for Watermarks Manipulation"
description: "Cloud REST API for watermarks management on images and documents of popular file formats within .NET applications."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: ".NET Watermark SDK"
        image: "/sdk/272x272/groupdocs_watermark-for-net.webp"
        product: "GroupDocs.Watermark"
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
            - link: "https://wiki.groupdocs.cloud/watermarkcloud/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-watermark-cloud/groupdocs-watermark-cloud-dotnet"
        link_learn: "https://docs.groupdocs.cloud/watermarkcloud/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Watermark Cloud SDK for .NET empowers you to programmatically manage text & image watermarks on a wide range of document formats including: PDF, Microsoft Word, Excel, PowerPoint, Visio, OpenDocument, JPEG, BMP, PNG, TIFF and many more.

      It supports working with all most demanded watermarking methods to let you add, remove, search and replace watermarks from images and documents of supported formats. The older watermarks already added inside the document can also be removed, no matter if they were added by third party tools. It’s easier to customize watermark formatting settings by adjusting text style, font, size, color or position with minimal lines or code.

      GroupDocs.Watermark Cloud SDK for .NET is built as a layer on the top of GroupDocs.Watermark Cloud REST API, allowing a higher level of abstraction so that you don't need to know the REST API to use this SDK.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Watermark Cloud SDK for .NET only requires .NET Framework.



        right:
          enable: true
          icon: "fab fa-cubes"
          title: ".NET Framework"
          content: |
            
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Watermark Cloud supports a number of document formats.

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
        content: "Search and delete already added watermarks from supported file formats"

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
        content: "Secured watermark management solution"

      

      
    more_feature:
      # more_feature_loop
      - title: "Add Text Watermark to the Document – C#"
        content: |
          
          
          ```cs
          //Get your App SID, App Key and Storage Name at https://dashboard.groupdocs.cloud (free registration is required).
          public class AddTextWatermarks
              {
                  public static void Run()
                  {
                      var configuration = new Configuration(Common.MyAppSid, Common.MyAppKey);
                      var apiInstance = new WatermarkApi(configuration);

                      try
                      {
                          var fileInfo = new FileInfo
                          {
                              FilePath = "documents/sample.docx",
                              StorageName = Common.MyStorage
                          };

                          var options = new WatermarkOptions()
                          {
                              FileInfo = fileInfo,
                              WatermarkDetails = new List
                              {
                                  new WatermarkDetails
                                  {
                                      TextWatermarkOptions = new TextWatermarkOptions
                                      {
                                          Text = "New watermark text",
                                          FontFamilyName = "Arial",
                                          FontSize = 12d,
                                      }
                                  }
                              }
                          };

                          var request = new AddRequest(options);

                          var response = apiInstance.Add(request);
                          Console.WriteLine("Resultant file path: " + response.Path);
                      }
                      catch (Exception e)
                      {
                          Console.WriteLine("Exception while calling WatermarkApi: " + e.Message);
                      }
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