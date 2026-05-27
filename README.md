Gaussian2Plane: Compact Plane Extraction from 3D Gaussian Splatting Scenes via Coplanarity-Guided Refinement


Planar primitives are fundamental geometric elements in man-made environments and play a crucial role in complex tasks such as building reconstruction and scene understanding. Recent advances in 3D Gaussian Splatting (3DGS) have enabled high-quality scene synthesis and fine-grained reconstruction for photogrammetric 3D modeling, but deriving a compact set of geometrically faithful planes from 3DGS scenes remains challenging, as their unstructured representation provides no explicit surfaces. Existing methods often derive local planar features or primitives first and obtain explicit planes through subsequent merging, making plane-set compactness difficult to integrate into geometric refinement and leading to fragmented or redundant plane sets. This paper proposes Gaussian2Plane, a coplanarity-guided continuous-discrete refinement method for compact plane extraction from 3DGS scenes. The key idea is to perform coplanarity-guided refinement under 3DGS-rendered geometric supervision, progressively consolidating redundant coplanar primitives into compact plane structures through continuous geometric optimization and periodic discrete identity-driven structural updates. This coupling enables geometric fidelity and plane-set compactness to be jointly optimized within the same refinement process. Gaussian2Plane first constructs an identity-aware planar scaffold from 3DGS-rendered geometry, providing initial planar coverage and plane-level identity priors, and then refines this scaffold into compact and geometrically consistent plane sets through coplanarity-guided refinement. Experiments on outdoor and indoor scenes show that our method produces more compact and complete plane sets than existing methods while maintaining comparable geometric accuracy, providing a reliable geometric basis for compact mesh reconstruction and scene understanding.
<img width="798" height="639" alt="image" src="https://github.com/user-attachments/assets/e9fdd537-e3a3-465d-a2ff-995559db1c04" />





 Input city model
<img width="975" height="1395" alt="image" src="https://github.com/user-attachments/assets/bb2374ea-b185-42fa-98cb-880bf6b19fcc" />





Application in compact mesh reconstruction.
<img width="874" height="532" alt="image" src="https://github.com/user-attachments/assets/c1832d98-b8ff-4178-a54b-c32ca043bb77" />


Extension to point-cloud inputs and application in compact mesh reconstruction
<img width="526" height="572" alt="image" src="https://github.com/user-attachments/assets/73594d46-022b-4b9a-8999-6a73e13fb846" />




