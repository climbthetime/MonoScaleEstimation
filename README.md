## Simple but Effective Scale Estimation for Monocular Visual Odometry in Road Driving Scenarios
Additional experimental results for the paper titled above.
### Abstract
In large scale environments, scale drift is a crucial problem of monocular visual SLAM. A common solution is to utilize the camera height, which can be obtained using the reconstructed 3D ground points~(3DGPs) from two successive frames, as prior knowledge.Increasing the number of 3DGPs by using more proceeding frames can be a natural extension of this solution to estimate a more precise camera height. However, merely employing multiple frames based on conventional methods is hard to be directly applicable in a real-world scenario because the vehicle motion and inaccurate feature matching inevitably cause large uncertainty and noisy 3DGPs. In this study, we propose an elaborate method to collect confident 3DGPs from multiple frames for robust scale estimation. First, we gather 3DGP candidates that can be seen in more than a predefined number of frames. To verify the 3DGP candidates, we filter out the 3D points at the exterior of the road region obtained by the deep-learning-based road segmentation model. In addition, we formulate an optimization problem constrained by a simple but effective geometric assumption that the normal vector of the ground plane lies in the null space of a movement vector of the camera center, and provide a closed-form solution. ORB-SLAM with the proposed scale estimation method achieves the average translation error with 1.19\% on the KITTI dataset, which outperforms the state-of-the-art conventional monocular visual 

*****************************************************************************************
#### Example of ATE results obtained using SEMK and GCSEMK for the sequences 00, 02-10.
![](https://lh3.googleusercontent.com/jJppO4bsvd80n1fjvw-bSXWWFSAw-08PYAh2ORA3h47R_17zt2BqQgMAeQIjtsSgnd5QjFNOADFc0uDdGwCZTn7pKfjXWT990jAKJr9P-TWe72-fEQYfoHDBN-2OEsVqUSv3Bee9OT1C5KVPLXavoHKmH_iDjvM8eIzyFKFsD9n1HZA3YkYYjgq9lBSfi7yrSNfTEMBjuq1hfZpjhxPEeQSuMMHofOTBGjVxcv87MndVjSSlkIueWYxNoHKTzwfHroJqq5IbB85FvH91uTeqnyNEIov-mUzYwas6ZulNL6F8EtrTLQE7vuDhxbJApq7uYJFchzO2kQFc7HZu8J0C9gJBjFlCvBh0GN2oNQcRPaIkNzu8usauIPaabjQXBB_Ngfk5n1cuJKwzQ63GyPEAIaN6VdmUI1tHvT46g-IHxSxseY3uW0ynCr72UZ1yIKARB9GGwvToBuAds4FWUUIgaGX2JDXcR-4zieyacmI3p89WOE5olnFAUa3HmHs6bxSJCAdOGYNGgDpy-6FAqXaUoE4JtWrC7M4xFB5WqmaFZrGDbS7gHQZdJwUaRWSXrRCFSQrnob9gDQR7Sy2_LB4yY0WvskGYIPBLI4i7Au-gBuXNIZJfQtuQNCUizEO_KHUV9zuCXpMxXrsVt3YEMg2LBBbbj8McTC93QeLHt70j2L8_9sUyELMwk6gZvKh_=w1340-h1928-no?authuser=0)

*****************************************************************************************
#### Recorded video for sequence 00, 02-10. The trajectory of ground truth, ORB-SLAM without loop closure and GCSEMK are shown in red, black, and blue respectively. The black sparse points are the reconstructed 3D points. The detected feature points on the ground region are shown as red square in the image.
##### Recorded video for sequence 00
{% include 00.html%}
##### Recorded video for sequence 02
{% include 02.html%}
##### Recorded video for sequence 03
will be available soon
##### Recorded video for sequence 04
will be available soon
##### Recorded video for sequence 05
will be available soon
##### Recorded video for sequence 06
will be available soon
##### Recorded video for sequence 07
{% include 07.html%}
##### Recorded video for sequence 08
will be available soon
##### Recorded video for sequence 09
will be available soon
##### Recorded video for sequence 10
will be available soon

*****************************************************************************************
#### The estimated camere trajectories using SEMK for sequence 00 and 02-10 in the KITTI benchmark
![](https://lh3.googleusercontent.com/pw/ACtC-3fpxjxGrH9vo3aunm7OQlyg-VUT-TtbkOlRomXZZIiFXR_U-j4NkRO6L-5oqwTL2A7WD6UmKX0O8d9IKFGLhk-NtVlWotDj4W-uBuGPvH55rFEC5FdX55SE2NgX7RbmSZ5epWd4J-wo-Bv7SEjdChKC=w682-h984-no?authuser=0)
![](https://lh3.googleusercontent.com/pw/ACtC-3fcM9mUw8NAds1as8qoTsAdJLfhA2VolYVrZ9Age-XeyCp13l_lC6sFWu09uOzvTUjTWbU0k4gRk6X6ryM0n3ej3LV71Q0GSVqalbTzy99E5eq3TNM_Xrb30QbCUy0CYaoTaetAoIQ13fJ-WrIWovm2=w682-h984-no?authuser=0)
#### The translation and rotation errors over different distance segment
![](https://lh3.googleusercontent.com/BOkRL2Sm2oUgHaetC5oFhA0MSoKMc58e64j2O4BxWC4qNFvD3cWRVpPNhrDKRm91myMLuZ7TGxwt34tU1q022MlPBJlS88fVVLihbSePPSaSzNYYpoi3V8y0cmbxT2Uji6-i8kKM8C0vb6Nh3cMSBPkkygfYwSClaYnfzkuYZBra3EBWBC79kSV0N1IcvSLinMndJly5e2M0EeeKsk91A9Tum0iBxP2qvpP6Y68eBtJKY9XoaMfY3ZmNv3hCFSgPBEUOxSaWnLo_8MRHmwepB4fLyjwkYQUkcBNh2sIw66NEArz2tui6ZeDkum633t9t-UPSoVtQx9RzzbDU-PBmBMO_QAXMu-acxRaCD8HpqqQa3sYA_3AdZXhPTxV3Qetv1XVUi7bOkSqIL9SNM5fH8pRjD_EUGg0T3Oq2VW6bTvmlnvygOshpH65ioiwE_MUKeucu6XEH5Pw2ghTC6Ca8-MHVFbbd8vqZFMdYovRZQZ0AOcuedYSJLFUE7x9jx20_GkWdK511TNCbbfdttpA0bq-dwTtK1USF2Oop11mOKS7FX5BpkAP4P_Z7jNHQgDM8pPRvEJe-YMT1T5oPCSwZ7X-udktUH-eiqhE7eG125OgoiOXPp4FkuaxgE1RgD1TS7LXN3vUZQd6fC8Ra6R3KpvCOWcF6DE1pDgQ16KDY_pXsQ4DPlgRxEjJGHEHW=w720-h1040-no?authuser=0)

#### The translation errors via |K| and delta
![](https://lh3.googleusercontent.com/fHll_t6daHB3CEmEF9U49CRDyLCQrBSPnCL-1zMgns8XovvGxkaBkOc2RD26bBqJnf-pQQcvUJft6jz8aeEWFyvqkAU--KUDlO9oh4-hjiSPSKOlzycnkqf6JBFlL4nD25ttlrHDjayWjVCR3OF6c25KXqV9lCxUttKQwOXRrbjF9E-sJM_tA6tTM3UoevCYAseXgF5OqP6No4TTb8c-0PO1EmpsG-0mD2mxcSLc0neYD2iEmT0wBBANI3rrkgrgInWtJqEAfMcnogbL935Ppkc3bPt-QOLF6jyxC3up5K7dOjBemNk46LbspNVkWGoqMKP-qKa41XKCuxtMLFnyixd-sS5AHhwfloEEV0dGl7wJ9Dj5epF3KdyHI0dAtt__GUnEIuXiNgEkxW3lHBqe02_GYWibWdUJ_h8QvdAv1N70chLJIVUkjRgUsk7Mu1U5jFj-uvoF607p5PxVaDvp8vjvJd27qPdT6Fs4ybJO-AVcpIo0cHyvbXp7V54swcOCmmNCizPB7GLOQnjMYHAO8T4BufjgWHz3TV0nG4-7uGXgm3Qwa2NYkUT8Ck3TZkBCGkMiU1z0D4PsDkcgejNXfaHdRRJTHi3H0BBZHq8Ae2BtjktKLwMFBvUC-_jB6SwSUBjvTM845IolO6Hh4tPt98O2nVCd_R9StuvHqa6VZmXzbYCIE19DInxRylkV=w2598-h1866-no?authuser=0)

