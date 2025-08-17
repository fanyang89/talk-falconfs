# FalconFS Technical Presentation

This is a technical presentation about FalconFS distributed file system, focusing on its innovative design for deep learning scenarios.

## Presentation Content

### Core Topics

- **FalconFS**: Distributed file system designed for large-scale deep learning pipelines
- **Production Validation**: Used in Huawei's autonomous driving system with 10,000 NPUs for one year
- **Performance Advantages**: 5.72× improvement in small file I/O, 12.81× improvement in deep learning training

### Main Chapters

1. **Background** - Challenges in deep learning scenarios
2. **Data Lake Technology** - Modern data management solutions
3. **Deep Learning Pipeline** - Autonomous driving training pipeline
4. **FalconFS Architecture** - Stateless client design
5. **Key Technologies** - Hybrid metadata indexing, lazy namespace replication
6. **Performance Evaluation** - MLPerf Storage Benchmark results

### Core Innovations

- **Stateless Client**: Removes client metadata caching, enables single-hop access
- **Hybrid Indexing**: Intelligent routing combining hash and path traversal
- **Concurrent Request Merging**: Reduces network round trips, improves training efficiency
- **Lazy Namespace Replication**: Avoids distributed transaction overhead

## Presentation Startup

```bash
# Install dependencies
pnpm install

# Start presentation
pnpm dev

# Visit http://localhost:3030
```

Edit [slides.md](./slides.md) to view slide content.

Built with Slidev, learn more at [official documentation](https://sli.dev/).
