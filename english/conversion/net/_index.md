---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Conversion"
product_tag: "conversion"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Document Converter Cloud SDK for PDF Word Excel HTML & Images"
head_description: ".NET Cloud SDK for Document and images conversion. Use REST APIs to convert between PDF, Word, Excel, PPTX, Visio, Project, HTML & email formats."

############################# Header ############################
title: ".NET Cloud SDK for Document Conversion"
description: "Build tools to convert documents and images of popular file formats back and forth using .NET Cloud SDK for document conversion & REST API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Conversion Cloud SDK for .NET"
        image: "/sdk/272x272/groupdocs_conversion-for-net.webp"
        product: "GroupDocs.Conversion"
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
            - link: "https://docs.groupdocs.cloud/conversion/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-dotnet"
        link_learn: "https://docs.groupdocs.cloud/conversion/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      The GroupDocs.Conversion Cloud SDK for .NET has been developed to help you get started with using our document conversion REST API, allowing to seamlessly convert your documents to any format you need. With this single API, you can convert back and forth between over 50 types of documents and images, including all Microsoft Office and OpenDocument file formats, PDF documents, HTML, CAD, raster images and many more.
    tabs:
      enable: true   
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Conversion Cloud for .NET has following SDK Requirements:

        right:
          enable: true
          icon: "fas fa-cubes"
          title: ".NET Framework"
          content: |
            

      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Conversion Cloud converts back and forth between a variety of documents and images.



        left:
          enable: true
          table:
            # table loop
            - title: "Convert From:"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP, OTS, ODG
                * **Microsoft Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLAM
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX, POT
                * **Visio‎**: VSD, VDX, VSS, VSX, VST, VTX, VSDX, VDW, VSSX, VSTX, VSDM, VSTM, VSSM
                * **Project**: MPP, MPT, MPX
                * **Microsoft OneNote**: ONE
                * **Email**: MSG, EML, EMLX
                * **Fixed Layout**: PDF, XPS
                * **Web**: HTML, MHT, MHTML
                * **AutoCAD**: DXF, DWG, DWT, STL, DWF, IFC
                * **Image files**: BMP, GIF, JPG, PNG, TIFF, multi-page TIFF, WebP, DjVu, SVG, DNG, DIB, JPC, JPEG-LS
                * **Metafile**: WMF, EMF
                * **Other**: TXT, CSV, XML, DICOM, TEX, MOBI, EPUB, ICO

        right:
          enable: true
          table:
            # table loop
            - title: "Convert To:"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP
                * **OpenDocument**:  XLS, XLSX, XLSM, XLSB, XLAM
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Metafiles**: WMF, EMF
                * **Image Files**: BMP, GIF, JPG, PNG, TIFF, multi-page TIFF, WebP, SVG, DNG, PSD
                * **Other**: PDF, EPUB, TXT, HTML‎

      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Conversion Cloud API while using your favorite language & platform.
        
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
    title: "Advanced Document Conversion API Features"

    feature:
      # feature loop
      - icon: "fas fa-retweet"
        content: "Convert across all common formats"

      # feature loop
      - icon: "fas fa-star"
        content: "Convert page by page or custom range of pages"

      # feature loop
      - icon: "fas fa-copy"
        content: "Watermark pages"
      
      # feature loop
      - icon: "fas fa-star"
        content: "Get high quality output files"

      # feature loop
      - icon: "fas fa-shield-alt"
        content: "Password protect output document"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"

      # feature loop
      - icon: "fas fa-list"
        content: "API explorer based on swagger collection"

      

    more_feature:
      # more_feature_loop
      - title: "Convert a Multitude of Document Formats"
        content: |
          GroupDocs.Conversion REST API has the capability to perform conversion on a number of document formats. The information about the formats supported by the API can be obtained by using the code mentioned below:
      
      # more_feature_loop
      - title: "Get a list of supported document formats - C#"
        content: |
          ```cs
          //Get your AppSID, AppKey and StorageName at https://dashboard.groupdocs.cloud (free registration is required).
          var configuration = new Configuration("AppSID", "AppKey");
          var apiInstance = new ConversionApi(configuration);

          // Convert Settings
          var settings = new ConvertSettings
          {
              StorageName = "StorageName",
              FilePath = "conversions/sample.docx",
              Format = "jpeg",
              ConvertOptions = convertOptions,
              OutputPath = "converted/"
          };
          // Convert to Specified Format
          List response = apiInstance.ConvertDocument(new ConvertDocumentRequest(settings));
          ```

      # more_feature_loop
      - title: "Get Started in No Time"
        content: "With GroupDocs.Conversion Cloud API, you can start converting your files right away as there is no need to install anything. The API is clearly documented and comes with SDKs and live examples for all major languages. Our GroupDocs.Conversion SDKs along with working examples hosted at Github helps our users to get started in no time."

      # more_feature_loop
      - title: "Security and Authentication"
        content: "The GroupDocs.Conversion Cloud API is secured and requires authentication. You need to register at GroupDocs Cloud and get the app access key ID (appSID) and app secret access key. Authenticated requests require a signature and AppSID query parameters or OAuth 2.0 authorization header."
      
      # more_feature_loop
      - title: "API Explorer"
        content: "The easiest way to try out GroupDocs.Conversion Cloud API right away in your browser is by using GroupDocs Cloud Web API explorer, which is a collection of Swagger documentation for the GroupDocs Cloud APIs.It allows you to effortlessly interact and try out every single operation our APIs exposes."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Conversion Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_conversion-for-curl.webp"
          product: "GroupDocs.Conversion"
          platform: "cURL"
          link: "/conversion/curl/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_conversion-for-net.webp"
          product: "GroupDocs.Conversion"
          platform: ".NET"
          link: "/conversion/net/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_conversion-for-java.webp"
          product: "GroupDocs.Conversion"
          platform: "Java"
          link: "/conversion/java/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_conversion-for-php.webp"
          product: "GroupDocs.Conversion"
          platform: "PHP"
          link: "/conversion/php/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_conversion-for-python.webp"
          product: "GroupDocs.Conversion"
          platform: "Python"
          link: "/conversion/python/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_conversion-for-ruby.webp"
          product: "GroupDocs.Conversion"
          platform: "Ruby"
          link: "/conversion/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_conversion-for-node.webp"
          product: "GroupDocs.Conversion"
          platform: "Node.js"
          link: "/conversion/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_conversion-for-android.webp"
          product: "GroupDocs.Conversion"
          platform: "Android"
          link: "/conversion/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---